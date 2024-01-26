
# UniqueToken - ERC20 Token

## Overview
`UniqueToken` is a Solidity contract for an ERC20 token with extended functionalities such as minting and burning. It is built using OpenZeppelin's secure and community-vetted contracts. The token is designed to provide a robust framework for token management, especially suitable for projects requiring a token with customizable supply.

## Features
- **ERC20 Standard**: Implements all standard functionalities of an ERC20 token.
- **Mintable**: The owner can mint new tokens.
- **Burnable**: Token holders can burn their tokens to reduce the total supply.
- **Ownership Management**: Utilizes OpenZeppelin's `Ownable` for managing ownership privileges.

## Contract Details
- **Name**: `UniqueToken`
- **Symbol**: `UTK`
- **Decimals**: Uses ERC20 standard decimals (default is 18).

## Functions
### Constructor
- `constructor(address initialOwner)`: Sets the initial owner and mints an initial supply to the deployer's address.

### Mint
- `mint(address to, uint256 amount)`: Allows the owner to mint new tokens to a specified address.

### Burn
- `burn(uint256 amount)`: Allows any token holder to burn their tokens.

### Transfer
- `transfer(address recipient, uint256 amount)`: Allows token holders to transfer their tokens to another address.

## Development and Testing
To work with this contract, you should have a development environment set up for Solidity and Ethereum smart contract development. This typically includes tools like Truffle or Hardhat, and a testing setup using Ganache or a similar local Ethereum network.

## Usage
1. **Deployment**: Deploy the contract to an Ethereum network. During deployment, specify the initial owner's address.
2. **Minting Tokens**: The owner can mint tokens by calling the `mint` function.
3. **Transferring Tokens**: Token holders can transfer tokens using the standard ERC20 `transfer` function.
4. **Burning Tokens**: Token holders can burn their tokens to reduce the total supply.


