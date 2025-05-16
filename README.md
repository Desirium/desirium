# Desirium 💫

A decentralized wishlist donation platform that enables seamless crypto donations, automatic token swaps, and USDC distribution.

This project consists of:
- 📜 Smart Contract
- 🧠 Backend Service (Node.js)
- 💻 Frontend Application (React)

---

## 🎯 Goal

The **Desirium** platform allows users to:
- Create unique **wishlists**.
- Receive **donations in any token** (including meme coins).
- Automatically **swap** incoming tokens to **USDC** using **PumpSwap Library**.
- **Apply platform fees** based on token type.
- Transfer the remaining **USDC to the wishlist wallet address**.

---

## 🧩 Project Structure

### 🔸Frontend
A React-based web application that allows users to create wishlists, connect their wallets, and make donations in any supported token. It handles token selection, liquidity check via pump.fun, swap flow, and visualizes transaction progress and history.

### 🔸Backend
A Node.js-based API that coordinates swap operations through the pump.fun Swap API, calculates and applies platform fees, manages transaction logs, and interfaces securely with the blockchain for donation execution.

### 🔸Smart Contracts
Solana smart contracts responsible for generating unique PDA wallets per wishlist, handling incoming token donations, executing swaps, applying fee logic (0.5% for $SOL, 1% for meme coins), and transferring USDC to the designated wishlist wallet.

