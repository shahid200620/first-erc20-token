# MyToken (MTK)

## Overview
MyToken is a simple ERC-20 token built on the Ethereum blockchain using Solidity.  
This project was created as a beginner smart-contract exercise to understand how fungible tokens work, how balances are tracked, and how token transfers and approvals function on-chain.

The contract follows the ERC-20 standard and was deployed and tested using Remix IDE on the JavaScript VM.

---

## Token Details
- Name: MyToken  
- Symbol: MTK  
- Decimals: 18  
- Total Supply: 1,000,000 MTK  
- Standard: ERC-20  

The entire initial supply is assigned to the contract deployer during deployment.

---

## Implemented Features
- Standard ERC-20 token structure  
- Token transfer between addresses  
- Balance tracking for all addresses  
- Allowance system using approve and transferFrom  
- Transfer and Approval event emission  
- Input validation for zero address and insufficient balance  
- Solidity 0.8.x safety checks  

---

## Contract Functions

### balanceOf(address)
Returns the token balance of a given address.

### transfer(address to, uint256 amount)
Transfers tokens from the caller to another address.

### approve(address spender, uint256 amount)
Allows another address to spend tokens on behalf of the owner.

### transferFrom(address from, address to, uint256 amount)
Allows an approved address to transfer tokens from one account to another.

### allowance(address owner, address spender)
Returns remaining approved tokens a spender can use.

---

## Deployment Steps (Remix IDE)

1. Open Remix: https://remix.ethereum.org  
2. Create file `MyToken.sol`  
3. Select Solidity compiler version 0.8.x  
4. Compile the contract  
5. Go to Deploy tab  
6. Choose environment: Remix VM  
7. Enter total supply in constructor  
8. Click Deploy  

---

## Testing Performed

The following tests were executed in Remix:

- Contract compiled successfully  
- Token deployed with correct supply  
- Initial balance assigned to deployer  
- Transfer between accounts successful  
- Approval granted to another account  
- transferFrom executed using allowance  
- Allowance decreased after transfer  
- Transfer and Approval events emitted  
- Invalid transfers to zero address rejected  
- Transfers exceeding balance rejected  

Screenshots of compilation, deployment, transfers, and events are included in the repository.

---

## Project Structure

first-erc20-token/
│
├── contracts/
│ └── MyToken.sol
│
├── screenshots/
│ ├── compilation.png
│ ├── deployment.png
│ ├── token-info.png
│ ├── transfer-test.png
│ ├── approval.png
│ ├── transferFrom-test.png
│ └── events.png
│
└── README.md


---

## What I Learned
Through this project I learned how ERC-20 tokens operate internally, how balances and allowances are stored using mappings, and how smart contracts are compiled, deployed, and tested using Remix IDE.  
I also understood the importance of event emission, validation checks, and standard interfaces for compatibility with wallets and exchanges.

---

## Tools Used
- Solidity  
- Remix IDE  
- Ethereum Virtual Machine (JavaScript VM)  
- Git & GitHub  

---

## Author
Shahid Mohammed
