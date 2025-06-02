# 🚀 Memecoin Launchpad on Neon EVM 

## 📝 Overview
This project showcases how to build a Memecoin Launchpad on the Neon EVM Devnet. It enables users to create and oversee memecoin tokens with help of Raydium, and leveraging Solidity smart contracts deployed on Neon EVM.

## Prerequisites

- Node.js (v16 or higher)
- A Solana wallet with SOL for deployment
- A Metamask wallet with NEON and wSOL for Deployment.
- Basic understanding of Solana and Ethereum development.

## Project Structure

```
├── contracts/         # Smart contract files
├── test/              # Deployment and support scripts
└── README.md          # Project documentation
```

### Features
- **MemeLaunchpad Contract:** Serves as the core contract for launching and managing tokens
- **BondingCurve:** Manages the mechanics of token allocation
- **Raydium Integration:** Facilitates the setup of liquidity pools

### Installation
```bash
# Initialize project
git clone https://github.com/Harshkumar62367/meme-launchpad.git
pnpm init
```

### Configuration
1. Create `.env` file in the root folder:
```env
PRIVATE_KEY_OWNER: ""
PRIVATE_KEY_SOLANA: ""
USER1_KEY: ""
```

2. Add `id.json` file in your root with Solana Private Key in json format and run
```
export ANCHOR_WALLET=./id.json
```
3. Run the below script to deploy the Meme Launchpad
```
npx hardhat test test/MemeLaunchpad/MemeLaunchpad.js --network neondevnet
```
## 🔗 Contract Addresses and Transactions

### Deployed Contracts and Key Transactions
- **MemeLaunchpad Contract**: [`0x7923Ffeed7a43B096ac291200E3CE68AfFbD4b98`](https://neon-devnet.blockscout.com/address/0x7923Ffeed7a43B096ac291200E3CE68AfFbD4b98)
- **BondingCurve used at**: [`0x0Fc6Ec7F9F06bd733913C1Fcd10BFc959a1F88DC`](https://neon-devnet.blockscout.com/address/0x0Fc6Ec7F9F06bd733913C1Fcd10BFc959a1F88DC)
- **Token Sale Tx**: [`0xa0f6aff8e4f45f2d0aa1582fb6195a1d59008d855d06c3c1d733e448b6c0fc4f`](https://neon-devnet.blockscout.com/tx/0xa0f6aff8e4f45f2d0aa1582fb6195a1d59008d855d06c3c1d733e448b6c0fc4f)
- **Buy Transaction (Not Reaching Funding Goal)**: [`0x15cdf83cf392b079c6961b11600cc82acd4bc08f9343ba713092b72f8c0cda46`](https://neon-devnet.blockscout.com/tx/0x15cdf83cf392b079c6961b11600cc82acd4bc08f9343ba713092b72f8c0cda46)
- **Buy Transaction (Reached Funding Goal)**: [`0x84db240e9dd2fab07989b0ed39eeb8d52a0cbe1f3f9fb354774fbea0034fb14c`](https://neon-devnet.blockscout.com/tx/0x84db240e9dd2fab07989b0ed39eeb8d52a0cbe1f3f9fb354774fbea0034fb14c)
- **Raydium Pool ID**: [`DJx1QFNbGtdesMgXX1xA7cpT6sSNdADK312kCfgk4Ea7`](https://solscan.io/account/DJx1QFNbGtdesMgXX1xA7cpT6sSNdADK312kCfgk4Ea7?cluster=devnet)
- **Locked LP Amount**: 14142135523n
- **NFT Account holding LP position**: [`AAPHG2PC6datYCdKszf3iMgeNpXwZ1CxUTEixVUoD5s9`](https://solscan.io/token/AAPHG2PC6datYCdKszf3iMgeNpXwZ1CxUTEixVUoD5s9?cluster=devnet)
- **Claim Token Sale Fee Tx**: [`0x922b36a94a663994a9f27c9fed5e0790ff0341dadfedbddd496b35835d318ae5`](https://neon-devnet.blockscout.com/tx/0x922b36a94a663994a9f27c9fed5e0790ff0341dadfedbddd496b35835d318ae5)
- **Collect Pool Fees Tx**: [`0x224333911b7a6b17818f6696cf5c129ab756bbdf90a9928062f4781d5b2b566f`](https://neon-devnet.blockscout.com/tx/0x224333911b7a6b17818f6696cf5c129ab756bbdf90a9928062f4781d5b2b566f)

