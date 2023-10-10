import { findAll } from 'solidity-ast/utils';
import { ASTIssue, InputType, Instance, IssueTypes, RegexIssue } from '../../types';
import { findEndLineFromFunctionName, findStartLineFromFunctionName, getStorageVariable, getStorageVariable_Type_AccessModifier_SRC, instanceFromLineNumber, instanceFromSRC, lineFromIndex, printit } from '../../utils';

const issue: ASTIssue = {
  regexOrAST: 'AST',
  type: IssueTypes.GAS,
  gas: 100,
  title: 'The result of a function call should be cached rather than re-calling the function',
  description: "The function calls in solidity are expensive. If the same result of the same function calls are to be used several times, the result should be cached to reduce the gas consumption of repeated calls.",
  detector: (files: InputType): Instance[] => {
    let instances: Instance[] = [];
    
    let functionNames: string[] = [];
    for (const file of files) {
        if (!file.ast) continue;
        for (const node of findAll('FunctionDefinition', file.ast)) {
            if (node.kind !== 'function') continue;

            if (!!node.returnParameters && !!node.returnParameters.parameters && node.returnParameters.parameters.length > 0) {
                functionNames.push(node.name);
            }
        }
    }
    for (const file of files) {
        if (!file.ast) continue;
        for (const node of findAll('FunctionDefinition', file.ast)) {
            let startLine = findStartLineFromFunctionName(file.content, node.name);
            let endLine = findEndLineFromFunctionName(file.content, node.name);

            let nLOC = 1;
            let lines = file.content.split("\n");
            let checkedFunctions: string[] = [];
            let comments = [];
            for (let line of lines) {
                let trimmedLine = line.trim();
                if (trimmedLine.startsWith("\/") || trimmedLine.startsWith("*")) 
                    continue;
                
                if (nLOC >= startLine && nLOC <= endLine) {
                    for (let funcName of functionNames) {
                        if (checkedFunctions.includes(funcName))
                            continue;
                        let counter = 0;

                        if (line.includes(funcName + "(")) {
                            let nLOC2 = 1;
                            for (let line2 of lines) {
                                if (nLOC2 >= startLine && nLOC2 <= endLine) {
                                    if (line2.includes(funcName + "("))
                                        counter++;
                                }
                                nLOC2++;
                                if (nLOC2 > endLine) break;
                            }
                            if (counter > 1) {
                                comments.push(
                                    '/// @audit `' + funcName + "` is called " + counter + " times"
                                )
                                checkedFunctions.push(funcName)
                            }
                        }

                    }

                }
                nLOC++;
                if (nLOC > endLine) break;
            }

            if (comments.length !== 0) {
                instances.push(instanceFromSRC(file, node.src, node.body?.src, comments));
            }
        }
    }
    return instances;
  }
}

export default issue;
