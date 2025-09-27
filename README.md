# Predix Protocol 🔮  
**The Future, Priced In — Powered by CLOBs.**

Predix is a **CLOB-based decentralized prediction market protocol** that enables users to trade on the outcomes of real-world events with the efficiency and transparency of an on-chain order book. Unlike AMM-based prediction markets, Predix uses a **Central Limit Order Book (CLOB)** design for deeper liquidity, tighter spreads, and more efficient price discovery.

---

## ✨ Key Features
- **CLOB-Powered Trading** – Place bids and asks directly in the order book for precise pricing.  
- **Event Outcome Tokens** – Each market creates tradable YES/NO tokens (or multiple outcomes).  
- **Decentralized Settlement** – Oracles (e.g., Chainlink, UMA) resolve event outcomes.  
- **Open Market Creation** – Anyone can propose new event markets.  
- **Transparent Matching Engine** – On-chain smart contracts guarantee fair matching of orders.  
- **Liquidity Incentives** – Makers earn fees for providing liquidity.  

---

## 🛠️ How Predix Works

1. **Market Creation**  
   - Alice creates a market: *“Will ETH be above $3,000 on Dec 31, 2025?”*  
   - The protocol deploys YES/NO outcome tokens linked to that event.  

2. **Trading on the CLOB**  
   - Traders submit **limit orders** (buy/sell) to the on-chain order book.  
   - Orders are matched based on **price-time priority**.  

3. **Oracle Resolution**  
   - At event maturity, a decentralized oracle confirms the outcome.  
   - Example: Chainlink reports ETH/USD price on Dec 31.  

4. **Settlement**  
   - Winning outcome token holders redeem tokens for **1 USDC per YES/NO share**.  
   - Losing tokens are burned.  

---

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) v18+  
- [Hardhat](https://hardhat.org/) or [Foundry](https://getfoundry.sh/)  
- [MetaMask](https://metamask.io/) or compatible Web3 wallet  

### Installation
```bash
# Clone the repo
git clone https://github.com/your-org/predix-protocol.git

# Navigate into the project
cd predix-protocol

# Install dependencies
npm install
