# Report


## Low Issues


Total <b>1</b> instance over <b>1</b> issue:

|ID|Issue|Instances|
|-|:-|:-:|
| [L-1](#L-1) | Solidity version 0.8.20 or above may not work on other chains due to PUSH0 | 1 |

## Non Critical Issues


Total <b>2</b> instances over <b>1</b> issue:

|ID|Issue|Instances|
|-|:-|:-:|
| [NC-1](#NC-1) | Redundant inheritance specifier | 2 |

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


## Non Critical Issues

<a name="NC-1"></a> 
#### [NC-1] Redundant inheritance specifier
The contracts below already extend the specified contract, so there is no need to list it in the inheritance list again.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: test.sol

// No need for GameContract to inherit from Initializable, Governor is already inherited from Initializable
13: contract GameContract is Governor , Initializable {

// No need for Test to inherit from Governor, GameContract is already inherited from Governor
// No need for Test to inherit from Initializable, GameContract is already inherited from Initializable
// No need for Test to inherit from Initializable, Governor is already inherited from Initializable
17: contract Test is GameContract, Governor , Initializable {

```

</details>

---

