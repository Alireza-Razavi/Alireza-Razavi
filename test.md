# Report


## Gas Optimizations


| |Issue|Instances|
|-|:-|:-:|
| [GAS-1](#GAS-1) | Use `calldata` instead of `memory` for function arguments that do not get mutated | 2 |
| [GAS-2](#GAS-2) | Use Custom Errors | 25 |
| [GAS-3](#GAS-3) | Don't use `SafeMath` once the solidity version is 0.8.0 or greater | 2 |
| [GAS-4](#GAS-4) | Long revert strings | 10 |
| [GAS-5](#GAS-5) | Functions guaranteed to revert when called by normal users can be marked `payable` | 15 |
| [GAS-6](#GAS-6) | Use != 0 instead of > 0 for unsigned integer comparison | 14 |
| [GAS-7](#GAS-7) | Using assembly to check for zero can save gas | 26 |
| [GAS-8](#GAS-8) | `internal` functions not called by the contract should be removed | 5 |


## Non Critical Issues


| |Issue|Instances|
|-|:-|:-:|
| [NC-1](#NC-1) | Custom errors has no error details | 1 |
| [NC-2](#NC-2) | Import declarations should import specific identifiers, rather than the whole file | 52 |
| [NC-3](#NC-3) | Consider moving `msg.sender` checks to `modifier`s | 9 |
| [NC-4](#NC-4) | Redundant inheritance specifier | 2 |
| [NC-5](#NC-5) | Visibility of state variables is not explicitly defined | 1 |
| [NC-6](#NC-6) | Event is missing `indexed` fields | 12 |
| [NC-7](#NC-7) | Functions not used internally could be marked external | 17 |


## Low Issues


| |Issue|Instances|
|-|:-|:-:|
| [L-1](#L-1) | Governance functions should be controlled by time locks | 4 |
| [L-2](#L-2) | Missing storage gap for upgradable contracts | 2 |
| [L-3](#L-3) | Solidity version 0.8.20 or above may not work on other chains due to PUSH0 | 1 |
| [L-4](#L-4) | Using zero as a parameter | 40 |
| [L-5](#L-5) | Zero address check in initializer | 4 |
| [L-6](#L-6) | Empty Function Body - Consider commenting why | 2 |
| [L-7](#L-7) | Initializers could be front-run | 2 |
| [L-8](#L-8) | Functions calling contracts/addresses with transfer hooks should be protected by reentrancy guard | 1 |
| [L-9](#L-9) | Unsafe ERC20 operation(s) | 1 |
| [L-10](#L-10) | Upgradable contracts need a constructor to lock the implementation contract when it is deployed | 2 |


## Medium Issues


| |Issue|Instances|
|-|:-|:-:|
| [M-1](#M-1) | Centralization Risk for trusted owners | 11 |

