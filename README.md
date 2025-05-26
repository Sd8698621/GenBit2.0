# 🚀 GenBit (GBT) Smart Contract

GenBit (GBT) is a custom ERC20 token with built-in **tokenomics**, **order book trading**, **liquidity management**, and **governance voting**, designed to simulate decentralized exchange dynamics on-chain without relying on traditional AMMs (Automated Market Makers).

---

## 📜 Features

### ✅ ERC20 Token (Upgradeable)
- Total supply: `21,000,000 GBT`
- Upgradeable via proxy pattern
- Uses OpenZeppelin's secure base contracts

### 💰 Tokenomics
- Tax system with dynamic rates (1%–4%) that **decrease with adoption**
- Portion of tax is **burned** to reduce supply
- Collected tax used for liquidity injection

### 🧾 Order Book System
- Users can place **Buy** and **Sell** orders at specific prices
- Orders are matched in FIFO order (first-in, first-out)
- Trades include tax and burning logic

### 🏦 Liquidity Mechanism
- Liquidity auto-injected when USDT reserve falls below a threshold
- Liquidity grows proportionally to adoption

### 🗳 Governance Voting
- Token holders with ≥ `1000 GBT` can vote on proposals
- One vote per address per proposal
- All votes are recorded on-chain

### 🔐 Security
- Uses `ReentrancyGuard` to protect against reentrancy attacks
- `Ownable` access control for critical functions

---

## 🔧 Tech Stack

- Solidity `^0.8.20`
- OpenZeppelin Upgradeable Contracts
- EVM-compatible (Ethereum, BSC, Polygon, etc.)
- Deployment-compatible with Hardhat, Foundry, Remix

---

## 🛠 Installation & Deployment (Hardhat)

### 1. Clone the repo

```bash
git clone https://github.com/Sd8698621/GenBit2.0.git
cd GenBit2.0
```
### 2. Install dependencies
### 3. Compile
### 4. Deploy
### 5. Verify on Etherscan (optional)

### ✍️ Key Contracts
### Contract	Description
GenBit.sol	Main ERC20 token with order book, governance, and tax logic

- 📈 Adoption Metrics
- Tax rate reduces over time as adoption increases (adoptionProgress)

- Burn rate and liquidity injection scale with usage

### 🛡 Security Notes
- Upgradeable contract: Must be deployed using a proxy (Transparent or UUPS)

- Emergency functions: Admin can withdraw tokens from the contract in emergencies

- Governance safeguards: One vote per wallet per proposal, minimum balance required


```
MIT License © 2025 GenBit Developers
```
## Contract Details: 
```
0xfe26cee81eea554db2ff74431c8d07f6dcd9ab77eb80b9940a00961d9e6abd6b
```
![Screenshot 2025-05-01 225622](https://raw.githubusercontent.com/Sd8698621/GenBit2.0/refs/heads/main/demo.png)
