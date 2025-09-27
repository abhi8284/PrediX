# PrediX Protocol 🔮
**The Future, Priced In.**

PrediX is a **CLOB-based decentralized prediction market protocol** where anyone can trade on the outcomes of real-world events.  
Unlike AMM-based markets, PrediX uses a **Central Limit Order Book (CLOB)** for precise pricing, deep liquidity, and efficient price discovery — similar to how traditional exchanges operate.

---

## 🌍 Why PrediX?

Prediction markets are powerful tools for:
- **Forecasting** – Crowdsourcing probabilities of real-world events.  
- **Hedging** – Traders can hedge risks against uncertain outcomes.  
- **Speculation** – Users profit from insights about future events.  
- **Governance** – DAOs and protocols can integrate **futarchy** (governance via prediction markets).  

PrediX makes these markets **transparent, decentralized, and accessible** to anyone with a crypto wallet.

---

## ✨ Core Features

- **CLOB Trading Engine** – Place bids/asks in a fully on-chain order book with price-time priority.  
- **Event Outcome Tokens** – Each market mints YES/NO tokens that represent potential outcomes.  
- **Oracle-Based Resolution** – Outcomes resolved by decentralized oracles (Chainlink, UMA, or custom).  
- **Trustless Settlement** – Winnings automatically distributed via smart contracts.  
- **Market Creation** – Any user can create new event markets (sports, politics, crypto prices, governance).  
- **Liquidity Incentives** – Makers earn fees for providing liquidity to the order book.  

---

## 🔄 How PrediX Works

1. **Market Creation**  
   - A creator proposes a new event (e.g., *“Will ETH > $3,000 by Dec 31, 2025?”*).  
   - Smart contracts deploy **YES** and **NO** outcome tokens.  

2. **Trading**  
   - Traders place limit or market orders on the CLOB.  
   - Matching engine pairs buyers and sellers based on **price-time priority**.  
   - Collateral (e.g., USDC) is locked in escrow until resolution.  

3. **Resolution**  
   - After event maturity, the Oracle confirms the outcome.  
   - Example: Chainlink reports ETH/USD at $3,100 → **YES wins**.  

4. **Settlement**  
   - Winning token holders redeem their outcome tokens for **1 USDC each**.  
   - Losing tokens are burned.  

---

## 🏗️ Architecture

### Smart Contracts
- **MarketFactory.sol** → Deploys new markets & outcome tokens.  
- **OrderBook.sol** → Handles bids/asks, order matching, and escrow.  
- **OracleModule.sol** → Connects to Chainlink / UMA for outcomes.  
- **SettlementEngine.sol** → Distributes winnings to correct outcome token holders.  

### Off-Chain Services
- **Relayer/Indexer (optional)** → Improves order discovery & UI responsiveness (like dYdX / Injective).  
- **Frontend App** → React + Next.js with Wagmi/RainbowKit for wallet connection.  

---

## 🧪 Example Trade

- Bob places a **limit buy**: 100 YES @ $0.45.  
- Carol places a **sell order**: 100 YES @ $0.45.  
- Orders match → Bob gets YES tokens, Carol receives USDC.  
- ETH ends above $3,000 → YES = 1 USDC → Bob redeems 100 USDC.  

---

## 🛠️ Tech Stack
- **Smart Contracts**: Solidity + Hardhat / Foundry  
- **Frontend**: React + Next.js + Wagmi / RainbowKit  
- **Backend (optional)**: Node.js + Postgres / Supabase (for metadata + order history)  
- **Oracles**: Chainlink, UMA, custom oracle modules  

---

## 📦 Planned Packages
- `@predix/contracts` → Core Solidity contracts  
- `@predix/sdk` → TypeScript SDK for dApp devs  
- `@predix/app` → Frontend reference dApp  

---

## 🌐 Vision
PrediX aims to become the **go-to decentralized prediction layer** for:  
- **DeFi protocols** → Integrating futarchy for governance decisions.  
- **Sports betting platforms** → Transparent, on-chain betting.  
- **Financial forecasting** → Markets on macroeconomic outcomes (e.g., inflation, rates).  
- **Crypto-native predictions** → Will BTC ETF be approved? Will ETH Flippening happen?  

---

## 🤝 Contributing
We welcome contributions!  
- Open issues for bugs or feature requests.  
- Submit PRs to improve the codebase.  
- Join our discussions on Discord to shape the protocol.  

---

## 📜 License
MIT License © 2025 PrediX Protocol
