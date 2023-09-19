# Report


## Non Critical Issues


| |Issue|Instances|
|-|:-|:-:|
| [NC-1](#NC-1) | Visibility of state variables is not explicitly defined | 1 |


## Low Issues


| |Issue|Instances|
|-|:-|:-:|
| [L-1](#L-1) | Solidity version 0.8.20 or above may not work on other chains due to PUSH0 | 1 |
| [L-2](#L-2) | Using zero as a parameter | 2 |
| [L-3](#L-3) | Initializers could be front-run | 1 |



## Non Critical Issues


<a name="NC-1"></a> 
#### [NC-1] Visibility of state variables is not explicitly defined
To avoid misunderstandings and unexpected state accesses, it is recommended to explicitly define the visibility of each state variable.

<details>

<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: test.sol

6: 	uint256 constant MAX_FUTURE_ROUND = 2**256 - 1;

```


</details>

---


## Low Issues


<a name="L-1"></a> 
#### [L-1] Solidity version 0.8.20 or above may not work on other chains due to PUSH0
Solidity version 0.8.20 or above uses the new [Shanghai EVM](https://blog.soliditylang.org/2023/05/10/solidity-0.8.20-release-announcement/#important-note) which introduces the PUSH0 opcode. This op code may not yet be implemented on all evm-chains or Layer2s, so deployment on these chains will fail. Consider using an earlier solidity version.

<details>

<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: test.sol

1: pragma solidity ^0.8.9;

```


</details>

---

<a name="L-2"></a> 
#### [L-2] Using zero as a parameter
Taking `0` as a valid argument in Solidity without checks can lead to severe security issues. A historical example is the infamous `0x0` address bug where numerous tokens were lost. This happens because 0 can be interpreted as an uninitialized `address`, leading to transfers to the 0x0 address, effectively burning tokens. Moreover, `0` as a denominator in division operations would cause a runtime exception. It's also often indicative of a logical error in the caller's code. It's important to always validate input and handle edge cases like `0` appropriately. Use `require()` statements to enforce conditions and provide clear error messages to facilitate debugging and safer code.

<details>

<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: test.sol

17: 		callme(address(0));

18: 		callme2(0);

```


</details>

---

<a name="L-3"></a> 
#### [L-3] Initializers could be front-run
Initializers could be front-run, allowing an attacker to either set their own values, take ownership of the contract, and in the best case forcing a re-deployment

<details>

<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: test.sol

16: 	function init() external {

```


</details>

---
