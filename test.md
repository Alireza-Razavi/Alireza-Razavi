# Report


## Gas Optimizations


| |Issue|Instances|
|-|:-|:-:|
| [GAS-1](#GAS-1) | Using assembly to check for zero can save gas | 1 |


## Non Critical Issues


| |Issue|Instances|
|-|:-|:-:|
| [NC-1](#NC-1) | Functions not used internally could be marked external | 1 |



## Gas Optimizations

### <a name="GAS-1"></a>
<details>
<summary>[GAS-1] Using assembly to check for zero can save gas</summary>
Using assembly to check for zero can save gas by allowing more direct access to the evm and reducing some of the overhead associated with high-level operations in solidity.

*Instances (1)*:
```solidity
File: test.sol

6: 		if (inputNumber == 0) {

```
</details>



## Non Critical Issues

### <a name="NC-1"></a>
<details>
<summary>[NC-1] Functions not used internally could be marked external</summary>

*Instances (1)*:
```solidity
File: test.sol

5: 	function my_function(uint256 inputNumber) public pure returns(bool) {

```
</details>

