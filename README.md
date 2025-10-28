
# 🎲 Lottery Smart Contract

A simple **Ethereum-based Lottery DApp** built with **Solidity**, where participants can enter by paying a fixed fee. The contract manager (creator) can pick a random winner who receives the total balance.

---

## 📜 Smart Contract Overview

### 🧩 Entities

* **Manager** — The contract creator who controls key functions.
* **Players** — Participants entering the lottery by paying **10 wei**.
* **Winner** — Randomly selected player who receives the total lottery balance.

---

## 💡 Project Highlights

✅ Participants can join the lottery by paying a **fixed amount (10 wei)**.
✅ Only the **manager** can view the contract balance or pick the winner.
✅ **Winner selection** is done using a pseudo-random hash (`keccak256`) with on-chain parameters.
✅ The **entire contract balance** is transferred to the winner, and the lottery resets for the next round.

---


## 🛠️ Tech Stack & Tools Used

| Component                   | Technology         |
| --------------------------- | ------------------ |
| **Smart Contract Language** | Solidity           |
| **Blockchain Network**      | Ethereum (Testnet) |
| **Wallet Integration**      | MetaMask           |
| **Testing Faucet**          | MegaETH Faucet     |
| **Development Environment** | Remix IDE          |

---

## 🚀 How to Deploy

1. Open [Remix IDE](https://remix.ethereum.org/).
2. Create a new file `Lottery.sol` and paste the contract code.
3. Compile using Solidity compiler version `0.8.x`.
4. Deploy the contract using the **Injected Provider** (MetaMask).
5. Use the **participate()**, **getBalance()**, and **pickWinner()** functions from the Remix interface.

---

## 🔮 Future Improvements

* 🧱 Create a **React.js + Web3.js** frontend for easy interaction.
* 💰 Allow variable participation fees.
* 🎯 Add event logs for better transparency (e.g., `PlayerJoined`, `WinnerDeclared`).
* 🌐 Deploy on **Ethereum Mainnet** or **Polygon** for real users.
