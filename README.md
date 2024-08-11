# BlockchainMessengerapp

BlockchainMessengerapp is a simple smart contract written in Solidity that allows the owner to update a message on the blockchain. It also keeps track of the number of times the message has been changed.

## Overview

This smart contract is designed to store a message on the Ethereum blockchain that can be updated only by the contract's owner. It also maintains a counter that tracks how often the message changes.

## Features

- **Owner-Only Access**: Only the owner of the contract can update the message.
- **Message Tracking**: The contract stores a message that can be publicly viewed.
- **Change Counter**: The contract tracks the number of times the message has been updated.

## Contract Details

The contract includes the following state variables:

- **owner**: The address of the contract owner (the one who deployed the contract).
- **theMessage**: A string that stores the current message.
- **changeCounter**: A uint that tracks the number of times the message has been updated.

### Functions

- **constructor()**: Initializes the contract by setting the `owner` to the address that deploys the contract.
- **updateTheMessage(string memory _newMessage)**: Allows the owner to update `theMessage`. It increments `changeCounter` each time the message is updated.

## Installation

To work with this contract, you'll need to use [Remix IDE](https://remix.ethereum.org/), an online Solidity IDE.

### Steps to Get Started

1. Open Remix IDE by navigating to [Remix IDE](https://remix.ethereum.org/).
2. Create a new file named `BlockchainMessengerapp.sol`.
3. Copy the contract code and paste it into the newly created file.
4. Compile the contract using the Solidity compiler version `0.8.15`.
5. Deploy the contract using the "JavaScript VM" or your preferred environment.

### Deploying the Contract

1. After compiling the contract, go to the "Deploy & Run Transactions" tab.
2. Select `BlockchainMessengerapp` from the dropdown.
3. Click the "Deploy" button.

### Interacting with the Contract

- **Check the Owner**: Use the `owner` function to see the contract owner's address.
- **View the Current Message**: Use the `theMessage` function to view the current message.
- **View the Change Counter**: Use the `changeCounter` function to see how many times the message has been updated.
- **Update the Message**: As the owner, enter a new message in the `updateTheMessage` input field and click the `transact` button.
