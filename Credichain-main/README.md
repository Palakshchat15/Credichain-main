# Credichain - School Admin System

EduLedger is a comprehensive school administration system designed to manage various aspects of an educational institution. It allows administrators to manage student records, payments, certifications, wallet, transactions, voting, and NFT achievements, all in one platform. EduLedger uses modern technologies to ensure a sleek and efficient experience for administrators.

---

## Table of Contents

- [Overview](#overview)
- [Core Features](#core-features)
- [Technologies Used](#technologies-used)
- [Installation Guide](#installation-guide)
- [Usage](#usage)
- [Smart Contracts](#smart-contracts)
- [Frontend Structure](#frontend-structure)
- [Technologies](#technologies)
- [Deployment](#deployment)
- [License](#license)
- [Contributing](#contributing)
- [Contact](#contact)

---

## Overview

Credichain offers a suite of tools that make managing school operations seamless and more efficient. The platform provides a centralized hub for administrators to manage everything from student data and payment processing to certifications and voting systems. It features a modern, responsive UI, integrated with a backend to handle complex functionalities.

One key aspect of the system is its integration with the **Hedera ecosystem**, which powers the blockchain-based features such as **NFT achievements** and **tokenization**.

Key Features:
- Student records
- Course registrations
- Payment processing
- Certificate issuance

**Key Advantages:**
✔ Transparent academic ledger  
✔ Immutable data storage  
✔ Secure authentication via Hedera DID  
✔ NFT-based certification  

**Live Demo:** [https://eduledger.netlify.app/](https://eduledger.netlify.app/)

---

## ✨ Core Features

| Feature             | Description                                   | Technology Used                 |
|---------------------|-----------------------------------------------|---------------------------------|
| Course Registration | Decentralized course enrollment               | Hedera Consensus Service        |
| Fee Payments        | Secure transaction processing                 | Hedera Token Service (HTS)      |
| NFT Certificates    | Tamper-proof digital credentials              | ERC-721 Smart Contracts         |
| DID Authentication | Privacy-preserving identity verification      | Hedera Decentralized Identity   |
| Academic Records    | Permanent, immutable transcripts               | Hedera File Service             |

---

## 🛠 Installation Guide

### Prerequisites
- Node.js ≥ v14
- npm/yarn
- Hardhat
- Hedera Testnet Account

### Setup Instructions

1. **Clone Repository**
```bash
git clone https://github.com/bram-me/Eduledger.git
cd Eduledger
Install Dependencies

bash
Copy
Edit
# Frontend
cd frontend && npm install

# Smart Contracts
cd contracts && npm install
Environment Configuration

bash
Copy
Edit
# Sample .env file
HEDERA_NETWORK=testnet
ACCOUNT_ID=0.0.xxxx
PRIVATE_KEY=xxxxxx
CONTRACT_ID=0.0.xxxx
🚀 Usage
Frontend Development
bash
Copy
Edit
cd frontend
npm start  # Starts React dev server
Smart Contract Deployment
bash
Copy
Edit
npx hardhat compile
npx hardhat run scripts/deploy.js --network hederaTestnet
Available Scripts
Command	Action
npm test	Run test suite
npm run build	Create production build
npx hardhat verify	Verify deployed contracts
🤖 Smart Contracts
Contract Architecture
solidity
Copy
Edit
// EduLedger.sol
contract EduLedger {
    function registerCourse(uint256 courseId) external payable;
    function issueCertificate(address student) external onlyAdmin;
}

// EduCertificateNFT.sol (ERC-721)
contract EduCertificateNFT {
    function mint(address to, string memory metadataURI) external;
}
Contract Addresses (Testnet)
Main Contract: 0.0.xxxx

NFT Contract: 0.0.xxxx

🌐 Frontend Structure
css
Copy
Edit
src/
├── components/
│   ├── Dashboard.jsx
│   ├── CourseRegistration.jsx
│   └── CertificateViewer.jsx
├── services/
│   ├── hedera.js
│   └── contractService.js
└── App.js
🔗 Technologies
Blockchain Stack
Hedera Hashgraph (HTS, HCS, HFS)

Solidity (v0.8.0+)

Hardhat

ethers.js

Frontend Stack
React.js

Material-UI

Axios

Web3.js

🚢 Deployment
Netlify Deployment
bash
Copy
Edit
npm run build
netlify deploy --prod
Hedera Mainnet
Update hardhat.config.js

Fund deployment account

Run deploy script with mainnet credentials

📜 License
MIT License
Copyright (c) 2025 EduLedger Team

🤝 Contributing
Fork the repository

Create your feature branch

Submit a pull request

📧 Contact
bramwelvasaka@gmail.com
