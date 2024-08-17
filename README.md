# MyToken Smart Contract

## Overview

`MyToken` is an ERC20-based smart contract implemented using the Solidity programming language. This contract allows for the minting and burning of tokens, with ownership control to restrict minting operations. The contract is built using OpenZeppelin's ERC20 and Ownable modules for added security and functionality.

## Features

- **ERC20 Standard**: Implements the standard ERC20 interface.
- **Minting**: The contract owner can mint new tokens to any specified address.
- **Burning**: Token holders can burn their own tokens, reducing the total supply.
- **Ownership**: Only the owner of the contract can mint new tokens.

## Prerequisites

- **Solidity**: ^0.8.24
- **Remix IDE**: This contract is developed and tested on the Remix IDE.
- **OpenZeppelin Contracts**: Uses OpenZeppelin's ERC20 and Ownable contracts.

## Installation

To deploy and interact with this contract, follow these steps:

1. **Open Remix IDE**: Visit [Remix IDE](https://remix.ethereum.org/).
2. **Create New File**: Create a new Solidity file (e.g., `MyToken.sol`).
3. **Copy Code**: Copy the contract code into the newly created file.
4. **Compile**: Select the appropriate compiler version (`0.8.24` or higher) and compile the contract.
5. **Deploy**: Choose the desired environment (e.g., JavaScript VM, Injected Web3) and deploy the contract.

## Contract Methods

### `mint(address to, uint256 amount)`

- **Description**: Mints new tokens and assigns them to the specified address.
- **Access Control**: Only the contract owner can call this function.
- **Parameters**:
  - `to`: The address to receive the newly minted tokens.
  - `amount`: The number of tokens to mint.

### `burn(uint256 amount)`

- **Description**: Burns a specified number of tokens from the caller's account, reducing the total supply.
- **Access Control**: Any token holder can call this function.
- **Parameters**:
  - `amount`: The number of tokens to burn.

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
