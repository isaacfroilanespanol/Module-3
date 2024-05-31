# Saac Token

## Overview

Saac is a simple ERC20 token contract developed on the Ethereum blockchain. It provides standard ERC20 token functionalities such as transferring, minting, and burning tokens. Additionally, it includes an access control mechanism to restrict certain functions to the contract owner.

## Features

- *Name*: Saac Token
- *Symbol*: SAAC
- *Decimals*: 18 (standard for most ERC20 tokens)
- *Initial Supply*: Specified during contract deployment

## Functions

### mint(address account, uint256 amount)

Mints a specified amount of tokens and assigns them to the provided account address. This function can only be called by the contract owner.

### burn(uint256 amount)

Burns a specified amount of tokens from the caller's balance.

### transfer(address recipient, uint256 amount)

Transfers a specified amount of tokens from the caller's balance to the recipient's address.

### transferFrom(address sender, address recipient, uint256 amount)

Transfers a specified amount of tokens from the sender's balance to the recipient's address. This function requires an allowance to be set by the sender allowing the caller to transfer tokens on their behalf.

## Access Control

The contract owner has exclusive access to certain functions, enforced by the onlyOwner modifier. Only the owner of the contract can mint new tokens.

## Usage

Deploy the contract specifying the desired name, symbol, and initial supply. Interact with the contract using a compatible Ethereum wallet or through smart contract interactions.
