Blockchain-Based Academic Certificate Verification & Credit Transfer System

(A Decentralized Academic Credential Platform using Blockchain)

🚀 Project Overview

This project is a Blockchain-powered Academic Certificate Management System designed to ensure tamper-proof certificate issuance, verification, and academic credit transfer as per NEP 2020 guidelines.

The platform provides secure credit transfer, certificate validation, and transparent student academic ledger tracking, ensuring credibility during placements, higher studies, and industry verification processes.

Blockchain-Based Academic Certificate Verification & Credit Transfer System

A decentralized academic credential system using blockchain, designed for tamper-proof certificate issuance, verification, and academic credit transfer.

🚀 Quick Start

Follow these steps to set up and run the project locally:

Clone the repository

git clone https://github.com/1rushikeshkale/Blockchain-Based-Academic-Certificate-Verification-and-Credit-Transfer-System.git
cd Blockchain-Based-Academic-Certificate-Verification-and-Credit-Transfer-System


Install dependencies
(Requires Node.js)

npm install


Start a Hardhat local development network (optional but recommended):

npx hardhat node


Deploy smart contracts
(Update script path if needed)

npx hardhat run scripts/deploy.js --network localhost


Run tests (if available):

npm test


(Currently, no test cases are configured.)

⚙️ Configuration

This project uses Hardhat for Ethereum development. Configuration details are maintained in hardhat.config.js.

For production deployments or testnet connections, use environment variables to store sensitive credentials.

Example .env file:
ALCHEMY_API_KEY="YOUR_ALCHEMY_API_KEY"
PRIVATE_KEY="YOUR_WALLET_PRIVATE_KEY"
ETHERSCAN_API_KEY="YOUR_ETHERSCAN_API_KEY"

Load variables in hardhat.config.js:
require('dotenv').config();
require("@nomicfoundation/hardhat-toolbox");

module.exports = {
  solidity: "0.8.19",
  networks: {
    sepolia: {
      url: `https://eth-sepolia.g.alchemy.com/v2/${process.env.ALCHEMY_API_KEY}`,
      accounts: [process.env.PRIVATE_KEY]
    }
  },
  etherscan: {
    apiKey: process.env.ETHERSCAN_API_KEY
  }
};

🎯 Key Objectives

✔ Secure and immutable certificate storage using Blockchain
✔ Prevent certificate forgery and fraud
✔ Automated academic credit calculation & transfer
✔ Trustless verification for employers and institutions
✔ Decentralized ledger for certificate and credit transparency

🖥️ System Modules

The platform consists of three core portals:

1️⃣ Admin / University Portal

Features:

Issue semester grade cards / academic certificates

Upload certificate documents to decentralized IPFS storage

Approve or reject student credit requests

View student certificates and earned credits

Burn certificate token if incorrect uploads occur

Manage blockchain admin wallets and minters (Hardhat accounts)

2️⃣ Student Portal

Features:

Register & login using PRN, email, and password

Submit internal academic credit requests

Upload external MOOC certificates:

NPTEL / SWAYAM

Coursera

edX

Automated credit calculation:

12 weeks = 3 credits

8 weeks = 2 credits

4 weeks = 1 credit

Track verified credits in real-time

Download approved certificates

3️⃣ Verification Portal

Used by companies, universities, and government bodies for secure validation.

Features:

Verify certificate via Token ID

Upload certificate file to verify authenticity

Validate student PRN and total earned credits

Secure academic record verification

No manual checking needed — blockchain guarantees authenticity.

👨‍💻 Tech Stack
Category	Technology
Blockchain	Solidity, Hardhat, MetaMask, EVM
Backend	Node.js, Express.js
Frontend	React.js, Tailwind CSS / Bootstrap
Database	MongoDB
Storage	IPFS / Pinata / NFT.Storage
Wallet	MetaMask
Dev Tools	Hardhat, Node.js, Alchemy / Infura
⚙️ How it Works
Admin issues certificate → 
Certificate stored on Blockchain → 
Token generated → 
IPFS hash stored → 
Student/Employer uploads certificate or token → 
Verified via Smart Contract

🔐 Security Features

Immutable blockchain records (cannot alter or delete)

Token-based identity for every certificate

Decentralized PDF/Image storage using IPFS

Smart contract permissions for minting and burning

🎓 Real-World Usage
User Type	Usage
Students	Submit MOOC certificates and track credits
Universities	Issue academic certificates and grade cards
Companies	Verify candidate certificates via blockchain
Govt. / Verification Bodies	Secure authentication of academic records
🧪 Blockchain & Testing
Local Blockchain Node
npx hardhat node

Smart Contract Deployment
npx hardhat run scripts/deploy.js --network localhost

📎 Future Enhancements

AI-based certificate OCR validation

NFT-based degree tokenization

QR-code powered verification portal

IPFS encryption for confidential documents

Mobile app support

University/NAAC analytics dashboard

📌 Screenshots
1. Admin Login ![Admin Login Page](https://github.com/1rushikeshkale/Blockchain-Based-Academic-Certificate-Verification-and-Credit-Transfer-System/blob/0bf8202d8be989239423fe89268259d9bf70b1dc/Admin%20Login%20Page.PNG?raw=true)

2. Issue Certificate Page ![Issue Certificate Page](https://github.com/1rushikeshkale/Blockchain-Based-Academic-Certificate-Verification-and-Credit-Transfer-System/blob/3ba9aa1d1c01b4e23d7316c0a5c2521c0b6f9f13/Issue%20Certificate.PNG?raw=true) 

3. Connect Metamask Page ![Connect Metamask Page](https://github.com/1rushikeshkale/Blockchain-Based-Academic-Certificate-Verification-and-Credit-Transfer-System/blob/3ba9aa1d1c01b4e23d7316c0a5c2521c0b6f9f13/Connect%20Metamask%20page.PNG?raw=true) 

4. Upload Certificate on Blockchain ![Upload Certificate on Blockchain](https://github.com/1rushikeshkale/Blockchain-Based-Academic-Certificate-Verification-and-Credit-Transfer-System/blob/3ba9aa1d1c01b4e23d7316c0a5c2521c0b6f9f13/Upload%20Certificate%20on%20Bloackchain.PNG?raw=true) 

5. Admin Approve Credit Page ![Admin Approve Credit Page](https://github.com/1rushikeshkale/Blockchain-Based-Academic-Certificate-Verification-and-Credit-Transfer-System/blob/3ba9aa1d1c01b4e23d7316c0a5c2521c0b6f9f13/Admin%20Approve%20Credit%20%20page.PNG?raw=true) 

6. Student Dashboard ![Student Dashboard](https://github.com/1rushikeshkale/Blockchain-Based-Academic-Certificate-Verification-and-Credit-Transfer-System/blob/3ba9aa1d1c01b4e23d7316c0a5c2521c0b6f9f13/Student%20Dashboard.PNG?raw=true) 

7. Verify Porta ![Verify Portal](https://github.com/1rushikeshkale/Blockchain-Based-Academic-Certificate-Verification-and-Credit-Transfer-System/blob/3ba9aa1d1c01b4e23d7316c0a5c2521c0b6f9f13/Verify%20Portal.PNG?raw=true) 

8. View or Verify Student Credit Using PRN Number ![View or Verify Student Credit Using PRN Number](https://github.com/1rushikeshkale/Blockchain-Based-Academic-Certificate-Verification-and-Credit-Transfer-System/blob/3ba9aa1d1c01b4e23d7316c0a5c2521c0b6f9f13/View%20or%20Verify%20Student%20Credit%20Using%20PRN%20Number.PNG?raw=true)



❤️ Credits

Developed by Rushikesh Kale
(Master of Computer Application)

📄 License

MIT License

⭐ Support the Project

Give the repository a ⭐ if you find it useful!

https://github.com/1rushikeshkale/MCAC11BlockchainProject

🙏 Contributing

We welcome contributions! To contribute:

Fork the repository

Create a feature or bugfix branch:

git checkout -b feature/your-feature-name


Make your changes

Commit with a clear message

Push to your fork

Create a Pull Request to the main branch

📬 Contact

📧 Email: 1rushikeshkale@gmail.com

🔗 LinkedIn: https://www.linkedin.com/in/1rushikeshkale/

“Blockchain for Education — ensuring trust, transparency, and authenticity.”
