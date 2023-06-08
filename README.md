# EtherWallet

A simple Ethereum wallet contract written in Solidity.

## Overview

EtherWallet is a basic Ethereum wallet contract that allows the owner to receive and withdraw Ether. The contract provides the following functionalities:

- The owner of the wallet can receive Ether from other addresses.
- Only the owner is allowed to withdraw Ether from the wallet.
- The owner can check the current balance of the wallet.

## Contract Details

The contract is written in Solidity version 0.8.0 and is for educational purposes only.

### Contract Structure

The main contract `EtherWallet` includes the following functions and modifiers:

- `constructor`: Initializes the contract and sets the owner as the deployer of the contract.
- `onlyOwner` modifier: Restricts access to functions only to the owner.
- `receive` function: Allows the contract to receive Ether from external addresses.
- `withdraw` function: Enables the owner to withdraw a specified amount of Ether from the wallet.
- `walletBalance` function: Retrieves the current balance of the wallet.
- `fallback` function: Reverts any calls to non-existent functions.

### Events

The contract emits the following event:

- `Log`: Logs the sender's address and the amount of Ether received or withdrawn.

### Usage

To use this contract, you can deploy it on the Ethereum network using a compatible development environment like Remix or Truffle. After deployment, you can interact with the contract using the following functions:

- `withdraw(uint _amount)`: Allows the owner to withdraw a specific amount of Ether from the wallet.
- `walletBalance()`: Retrieves the current balance of the wallet.

Please note that the contract requires you to be the owner in order to withdraw Ether. Also, remember to handle any reverts or failed transactions when using the contract functions.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
