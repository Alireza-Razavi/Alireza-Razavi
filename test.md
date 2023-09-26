# Report


## Low Issues


Total <b>2</b> instances over <b>1</b> issue:

|ID|Issue|Instances|
|-|:-|:-:|
| [L-1](#L-1) | Solidity version 0.8.20 or above may not work on other chains due to PUSH0 | 2 |

## Non Critical Issues


Total <b>24</b> instances over <b>18</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [NC-1](#NC-1) | Contract declarations should have NatSpec `@author` annotations | 2 |
| [NC-2](#NC-2) | Consider adding formal verification proofs | 1 |
| [NC-3](#NC-3) | Contracts should have full test coverage | 1 |
| [NC-4](#NC-4) | Convert simple `if` statements to ternary expressions | 1 |
| [NC-5](#NC-5) | Solidity version is different in some files | 2 |
| [NC-6](#NC-6) | Enable IR-based code generation | 1 |
| [NC-7](#NC-7) | Large or complicated code bases should implement invariant tests | 1 |
| [NC-8](#NC-8) | Missing zero address check in functions with address parameters | 1 |
| [NC-9](#NC-9) | NatSpec documentation for contract is missing | 2 |
| [NC-10](#NC-10) | NatSpec documentation for function is missing | 1 |
| [NC-11](#NC-11) | Missing NatSpec `@param` | 1 |
| [NC-12](#NC-12) | Public variable declarations should have NatSpec descriptions | 1 |
| [NC-13](#NC-13) | NatSpec `@return` is missing | 1 |
| [NC-14](#NC-14) | Redundant inheritance specifier | 1 |
| [NC-15](#NC-15) | State variables should include comments | 1 |
| [NC-16](#NC-16) | Contract declarations should have NatSpec `@title` annotations | 2 |
| [NC-17](#NC-17) | Solidity compiler version is not fixed | 2 |
| [NC-18](#NC-18) | Use the latest solidity version for deployment | 2 |

## Gas Optimizations


Total <b>9</b> instances over <b>5</b> issues:

|ID|Issue|Instances|Gas|
|-|:-|:-:|:-:|
| [GAS-1](#GAS-1) | Consider activating via-ir for deploying | 1 | - |
| [GAS-2](#GAS-2) | Newer versions of solidity are more gas efficient | 2 | - |
| [GAS-3](#GAS-3) | Reduce gas usage by moving to Solidity 0.8.19 or later | 2 | 2000 |
| [GAS-4](#GAS-4) | Use a more recent version of solidity | 2 | - |
| [GAS-5](#GAS-5) | Usage of `int`s/`uint`s smaller than 32 bytes incurs overhead | 2 | 110 |

## Low Issues

<a name="L-1"></a> 
### [L-1] Solidity version 0.8.20 or above may not work on other chains due to PUSH0
Solidity version 0.8.20 or above uses the new [Shanghai EVM](https://blog.soliditylang.org/2023/05/10/solidity-0.8.20-release-announcement/#important-note) which introduces the PUSH0 opcode. This op code may not yet be implemented on all evm-chains or Layer2s, so deployment on these chains will fail. Consider using an earlier solidity version.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: test.sol

1: pragma solidity ^0.8.9;

```

```solidity
File: test1.sol

1: pragma solidity ^0.8.10;

```

</details>

---


## Non Critical Issues

<a name="NC-1"></a> 
### [NC-1] Contract declarations should have NatSpec `@author` annotations

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: test.sol

5: contract Initializable {

```

```solidity
File: test1.sol

4: contract test1 {

```

</details>

---

<a name="NC-2"></a> 
### [NC-2] Consider adding formal verification proofs
Formal verification is the act of proving or disproving the correctness of intended algorithms underlying a system with respect to a certain formal specification/property/invariant, using formal methods of mathematics.

Some tools that are currently available to perform these tests on smart contracts are [SMTChecker](https://docs.soliditylang.org/en/latest/smtchecker.html) and [Certora Prover](https://www.certora.com/).

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity

Global finding

```

</details>

---

<a name="NC-3"></a> 
### [NC-3] Contracts should have full test coverage
While 100% code coverage does not guarantee that there are no bugs, it often will catch easy-to-find bugs, and will ensure that there are fewer regressions when the code invariably has to be modified. Furthermore, in order to get full coverage, code authors will often have to re-organize their code so that it is more modular, so that each component can be tested separately, which reduces interdependencies between modules and layers, and makes for code that is easier to reason about and audit.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity

Global finding

```

</details>

---

<a name="NC-4"></a> 
### [NC-4] Convert simple `if` statements to ternary expressions
Converting some if statements to ternaries (such as `z = (a < b) ? x : y`) can make the code more concise and easier to read.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: test.sol

19: 		if (x == address(0x0)) {
    			ppp = 0x1;
    		}
    		else {
    			ppp = 0x2;

```

</details>

---

<a name="NC-5"></a> 
### [NC-5] Solidity version is different in some files

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: test.sol

1: pragma solidity ^0.8.9;

```

```solidity
File: test1.sol

1: pragma solidity ^0.8.10;

```

</details>

---

<a name="NC-6"></a> 
### [NC-6] Enable IR-based code generation
The IR-based code generator was introduced with an aim to not only allow code generation to be more transparent and auditable but also to enable more powerful optimization passes that span across functions. You can enable it on the command line using `--via-ir` or with the option `{"viaIR": true}`. This will take longer to compile, but you can just simple test it before deploying and if you got a better benchmark then you can add --via-ir to your deploy command More on: https://docs.soliditylang.org/en/v0.8.17/ir-breaking-changes.html

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity

Global finding

```

</details>

---

<a name="NC-7"></a> 
### [NC-7] Large or complicated code bases should implement invariant tests
This includes: large code bases, or code with lots of inline-assembly, complicated math, or complicated interactions between multiple contracts. Invariant fuzzers such as Echidna require the test writer to come up with invariants which should not be violated under any circumstances, and the fuzzer tests various inputs and function calls to ensure that the invariants always hold. Even code with 100% code coverage can still have bugs due to the order of the operations a user performs, and invariant fuzzers may help significantly.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity

Global finding

```

</details>

---

<a name="NC-8"></a> 
### [NC-8] Missing zero address check in functions with address parameters
Adding a zero address check for each address type parameter can prevent errors.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: test.sol

/// Missing zero check for `x`
18: 	function ttT(address x) external returns(uint8){

```

</details>

---

<a name="NC-9"></a> 
### [NC-9] NatSpec documentation for contract is missing
e.g. `@dev` or `@notice`, and it must appear above the contract definition braces in order to be identified by the compiler as NatSpec.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: test.sol

5: contract Initializable {

```

```solidity
File: test1.sol

4: contract test1 {

```

</details>

---

<a name="NC-10"></a> 
### [NC-10] NatSpec documentation for function is missing
It is recommended that Solidity contracts are fully annotated using NatSpec for all public interfaces (everything in the ABI). It is clearly stated in the Solidity official documentation. In complex projects such as DeFi, the interpretation of all functions and their arguments and returns is important for code readability and auditability.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: test.sol

18: 	function ttT(address x) external returns(uint8){

```

</details>

---

<a name="NC-11"></a> 
### [NC-11] Missing NatSpec `@param`
Some functions have an incomplete NatSpec: add a `@param` notation to describe the function parameters to improve the code documentation.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: test.sol

/// Missing @param for x
18: 	function ttT(address x) external returns(uint8){

```

</details>

---

<a name="NC-12"></a> 
### [NC-12] Public variable declarations should have NatSpec descriptions

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: test.sol

17: 	uint8 public ppp;

```

</details>

---

<a name="NC-13"></a> 
### [NC-13] NatSpec `@return` is missing
It is recommended that Solidity contracts are fully annotated using NatSpec

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: test.sol

18: 	function ttT(address x) external returns(uint8){

```

</details>

---

<a name="NC-14"></a> 
### [NC-14] Redundant inheritance specifier
The contracts below already extend the specified contract, so there is no need to list it in the inheritance list again.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: test.sol

/// No need for GameContract to inherit from Initializable, Governor is already inherited from Initializable
11: contract GameContract is Governor , Initializable {

```

</details>

---

<a name="NC-15"></a> 
### [NC-15] State variables should include comments
Consider adding some comments on critical state variables to explain what they are supposed to do: this will help for future code reviews.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: test.sol

17: 	uint8 public ppp;

```

</details>

---

<a name="NC-16"></a> 
### [NC-16] Contract declarations should have NatSpec `@title` annotations
Some contract definitions have an incomplete NatSpec: add a `@title` notation to describe the contract to improve the code documentation.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: test.sol

5: contract Initializable {

```

```solidity
File: test1.sol

4: contract test1 {

```

</details>

---

<a name="NC-17"></a> 
### [NC-17] Solidity compiler version is not fixed
To prevent the actual contracts deployed from behaving differently depending on the compiler version, it is recommended to use a fixed solidity version.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: test.sol

1: pragma solidity ^0.8.9;

```

```solidity
File: test1.sol

1: pragma solidity ^0.8.10;

```

</details>

---

<a name="NC-18"></a> 
### [NC-18] Use the latest solidity version for deployment
Upgrading to a newer Solidity release can optimize gas usage, take advantage of new features and improve overall contract efficiency. Where possible, based on compatibility requirements, it is recommended to use newer/latest solidity version to take advantage of the latest optimizations and features.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: test.sol

1: pragma solidity ^0.8.9;

```

```solidity
File: test1.sol

1: pragma solidity ^0.8.10;

```

</details>

---


## Gas Optimizations

<a name="GAS-1"></a> 
### [GAS-1] Consider activating via-ir for deploying
By using `--via-ir` or `{"viaIR": true}`, the compiler is able to use more advanced [multi-function optimizations](https://docs.soliditylang.org/en/v0.8.17/ir-breaking-changes.html#solidity-ir-based-codegen-changes), for extra gas savings.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity

Global finding

```

</details>

---

<a name="GAS-2"></a> 
### [GAS-2] Newer versions of solidity are more gas efficient
The solidity language continues to pursue more efficient gas optimization schemes. Adopting a newer version of solidity can be more gas efficient.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: test.sol

1: pragma solidity ^0.8.9;

```

```solidity
File: test1.sol

1: pragma solidity ^0.8.10;

```

</details>

---

<a name="GAS-3"></a> 
### [GAS-3] Reduce gas usage by moving to Solidity 0.8.19 or later
Solidity version 0.8.19 introduced a number of gas optimizations, refer to the [Solidity 0.8.19 Release Announcement](https://soliditylang.org/blog/2023/02/22/solidity-0.8.19-release-announcement/) for details.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: test.sol

1: pragma solidity ^0.8.9;

```

```solidity
File: test1.sol

1: pragma solidity ^0.8.10;

```

</details>

---

<a name="GAS-4"></a> 
### [GAS-4] Use a more recent version of solidity
- Use a solidity version of at least 0.8.2 to get simple compiler automatic inlining.
- Use a solidity version of at least 0.8.3 to get better struct packing and cheaper multiple storage reads.
- Use a solidity version of at least 0.8.4 to get custom errors, which are cheaper at deployment than revert()/require() strings.
- Use a solidity version of at least 0.8.10 to have external calls skip contract existence checks if the external call has a return value.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: test.sol

1: pragma solidity ^0.8.9;

```

```solidity
File: test1.sol

1: pragma solidity ^0.8.10;

```

</details>

---

<a name="GAS-5"></a> 
### [GAS-5] Usage of `int`s/`uint`s smaller than 32 bytes incurs overhead
Using `int`s/`uint`s smaller than 32 bytes may cost more gas. This is because the EVM operates on 32 bytes at a time, so if an element is smaller than 32 bytes, the EVM must perform more operations to reduce the size of the element from 32 bytes to the desired size.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: test.sol

17: 	uint8 public ppp;

18: 	function ttT(address x) external returns(uint8){

```

</details>

---

