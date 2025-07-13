# 🚀 FUTURE_BC_02 – ERC-20 Token on BNB Testnet

This repository contains the code and documentation for **Task 2** of the **Future Interns Blockchain & Crypto Internship**. In this task, I developed and deployed a custom ERC-20 token using Solidity on the **BNB Smart Chain Testnet**.

---

## 📌 Overview

- **Internship Track**: Blockchain & Crypto
- **Task**: Write and deploy an ERC-20 or BEP-20 token on a testnet.
- **Technology Used**: Solidity, Remix IDE, MetaMask, BNB Testnet
- **Standard**: ERC-20 (OpenZeppelin)
- **Blockchain**: BNB Smart Chain Testnet

---

## 🔧 Tech Stack

| Tool        | Purpose                                  |
|-------------|-------------------------------------------|
| Solidity    | Smart contract development                |
| Remix IDE   | Writing, compiling, and deploying contract |
| MetaMask    | Wallet and Web3 provider                  |
| BNB Faucet  | Get test BNB for deployment               |
| OpenZeppelin| ERC-20 standard implementation            |
| GitHub      | Project and code documentation            |

---

## 🧠 What I Did

- Installed and configured **MetaMask** with the BNB Smart Chain Testnet.
- Wrote an **ERC-20** token smart contract using **OpenZeppelin**'s implementation.
- Deployed the contract using **Remix IDE** on the **BNB Testnet**.
- Verified contract deployment using **BscScan Testnet**.
- Captured all key screenshots and documented the process in this repo.

---

## 🔐 Token Details

| Attribute       | Value              |
|------------------|-------------------|
| **Token Name**   | MyToken           |
| **Token Symbol** | MTK               |
| **Total Supply** | 1,000,000 MTK     |
| **Decimals**     | 18                |
| **Deployed On**  | BNB Testnet       |


> Replace the contract address with your actual deployed address.

---

## 📂 Contract Code

The token is based on the standard OpenZeppelin ERC-20 implementation:

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20.sol";

contract MyToken is ERC20 {
    constructor(uint256 initialSupply) ERC20("MyToken", "MTK") {
        _mint(msg.sender, initialSupply * 10 ** decimals());
    }
}
