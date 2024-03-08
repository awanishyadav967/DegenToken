# Degen Token (ERC-20): Unlocking the Future of Gaming

## Overview

Welcome to the Degen Token (ERC-20) project! This Ethereum-based smart contract is deployed on the FUJI testnet and aims to create fungible tokens that can be used for gaming-related rewards. The contract adheres to the ERC-20 standard and provides essential functionalities like token minting, transfer, redemption, burning, balance checking, and more.

## Getting Started

To run this contract, follow the steps below:

1. Visit [Remix](https://remix.ethereum.org/) - an online Solidity IDE.
2. Create a new file with a .sol extension.
3. Copy and paste the provided code into the file.
4. Ensure the compiler version is set to "0.8.9" or a compatible version.
5. Compile the code using the "Solidity Compiler" tab.
6. Deploy the contract using the "Deploy & Run Transactions" tab.

## Contract Features

### Minting Tokens

- The contract allows the owner to mint new tokens using the `mint` function.

### Transferring Tokens

- Token holders can transfer tokens to other addresses through the `transfer` function.

### Redeeming Rewards

- Users can redeem rewards using the `claimReward` function, provided they have enough tokens.

### Burning Tokens

- The owner can burn tokens using the `burn` function.

### Checking Balances

- The contract supports checking token balances and available rewards.

### Reward System

- The contract features a reward system with predefined rewards and associated costs.

## Rewards

- Official Degen NFT - 50 tokens
- Merchandise - 100 tokens
- Credits - 100 tokens

## Additional Information

- The contract includes a struct for rewards, a mapping to track claimed rewards, and functions to interact with the contract.

## Usage Example

```solidity
// Example of interacting with the contract
DegenToken token = DegenToken(contractAddress);
token.mint(addressTo, amount);
token.transfer(anotherAddress, transferAmount);
token.claimReward(rewardIndex);
token.burn(addressFrom, burnAmount);
