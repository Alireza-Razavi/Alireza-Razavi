# Report


## Low Issues


Total <b>2</b> instances over <b>1</b> issue:

|ID|Issue|Instances|
|-|:-|:-:|
| [L-1](#L-1) | Solidity version 0.8.20 or above may not work on other chains due to PUSH0 | 2 |

## Non Critical Issues


Total <b>8</b> instances over <b>5</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [NC-1](#NC-1) | Contract declarations should have NatSpec `@author` annotations | 2 |
| [NC-2](#NC-2) | NatSpec documentation for contract is missing | 2 |
| [NC-3](#NC-3) | Redundant inheritance specifier | 1 |
| [NC-4](#NC-4) | Contract declarations should have NatSpec `@title` annotations | 2 |
| [NC-5](#NC-5) | Names of `private`/`internal` functions should be prefixed with an underscore | 1 |

## Gas Optimizations


Total <b>1</b> instance over <b>1</b> issue:

|ID|Issue|Instances|
|-|:-|:-:|
| [GAS-1](#GAS-1) | `internal` functions not called by the contract should be removed | 1 |

## Low Issues

<a name="L-1"></a> 
#### [L-1] Solidity version 0.8.20 or above may not work on other chains due to PUSH0
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

1: pragma solidity ^0.8.9;

```

</details>

---


## Non Critical Issues

<a name="NC-1"></a> 
#### [NC-1] Contract declarations should have NatSpec `@author` annotations

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
#### [NC-2] NatSpec documentation for contract is missing
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

<a name="NC-3"></a> 
#### [NC-3] Redundant inheritance specifier
The contracts below already extend the specified contract, so there is no need to list it in the inheritance list again.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: test.sol

// No need for GameContract to inherit from Initializable, Governor is already inherited from Initializable
11: contract GameContract is Governor , Initializable {

```

</details>

---

<a name="NC-4"></a> 
#### [NC-4] Contract declarations should have NatSpec `@title` annotations
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

<a name="NC-5"></a> 
#### [NC-5] Names of `private`/`internal` functions should be prefixed with an underscore
It is recommended by the [Solidity Style Guide](https://docs.soliditylang.org/en/v0.8.20/style-guide.html#underscore-prefix-for-non-external-functions-and-variables)

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: test1.sol

5: 	function test() internal view returns(uint256) {

```

</details>

---


## Gas Optimizations

<a name="GAS-1"></a> 
#### [GAS-1] `internal` functions not called by the contract should be removed
If the functions are required by an interface, the contract should inherit from that interface and use the `override` keyword

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: test1.sol

5: 	function test() internal view returns(uint256) {

```

</details>

---

