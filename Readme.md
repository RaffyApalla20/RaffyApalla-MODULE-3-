# Module3Assessment

# Overview

Module3Assessment is a custom ERC20 token built on the Ethereum blockchain. The token is named "Raffy" with the symbol "Raf". It leverages OpenZeppelin's implementation of ERC20 and Ownable contracts to ensure security and functionality. This contract includes additional custom events and functions for transferring, burning, and minting tokens.

# Functions

### constructor(address initialOwner, uint256 initialSupply)

Initializes the token contract with the specified owner and initial supply.

- initialOwner: The address of the initial owner of the contract.
- initialSupply: The initial supply of tokens.

### transferAmount(address recipient, uint256 amount) public virtual returns (bool)

Transfers tokens from the caller's account to the specified recipient and emits a custom transfer event.

- recipient: The address of the recipient.
- amount: The amount of tokens to transfer.
- Returns true if the transfer was successful.

### burnAmount(uint256 amount) public

Burns a specified amount of tokens from the caller's account and emits a burn event.

- amount: The amount of tokens to burn.

### mintAmount(address to, uint256 amount) public onlyOwner

Mints new tokens to the specified address and emits a mint event. This function can only be called by the owner.

- to: The address to receive the newly minted tokens.
- amount: The amount of tokens to mint.

# Remix IDE

This contract is designed to be used and tested in the Remix IDE, a powerful tool for developing, deploying, and managing smart contracts on the Ethereum blockchain. To use this contract in Remix IDE:

1. Open the Remix IDE in your web browser: [Remix IDE](https://remix.ethereum.org/)
2. Create a new file and copy the contract code into the file.
3. Compile the contract using the Solidity compiler.
4. Deploy and interact with the contract using the Remix interface.

# Owner

This contract is developed and maintained by Raffy Apalla.

# License

This project is licensed under the MIT License.

// SPDX-License-Identifier: MIT
Remix - Ethereum IDE
