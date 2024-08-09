Certainly! Here’s the revised README file without code snippets included in between:

---

# IndoorGameToken

## Overview

`IndoorGameToken` is a smart contract designed for a token-based system within a game environment. It implements the ERC20 token standard, allowing users to acquire and spend tokens for in-game items of varying levels. The contract includes functionalities for minting, burning, transferring tokens, and redeeming tokens for items.

## Features

- **ERC20 Token:** Implements the standard ERC20 token functionality.
- **Ownership Control:** Only the contract owner has the ability to mint new tokens.
- **Item Redemption:** Users can redeem tokens to acquire in-game items.
- **Token Burning:** Users can burn tokens from their balance.
- **Token Transfer:** Users can transfer tokens to other addresses.

## Contract Details

### Dependencies

The contract depends on OpenZeppelin's ERC20 and Ownable contracts.

### Constructor

- `constructor(address initialOwner)`: Initializes the token with the specified initial owner and sets up the token name ("GameTokens") and symbol ("GAMETOK").

### Functions

- **`mintTokens`**: Allows the contract owner to mint new tokens to a specified address.
- **`burnTokens`**: Allows users to burn tokens from their own balance.
- **`redeemGameToken`**: Allows users to redeem tokens for in-game items, burning the necessary amount of tokens and emitting an event.
- **`transferGameTokens`**: Enables users to transfer tokens to another address.

## Example Usage

1. **Mint Tokens**: The owner can mint tokens for a specific address.
2. **Burn Tokens**: Users can burn a specified amount of their tokens.
3. **Redeem Game Token**: Users can redeem tokens for a specific in-game item.
4. **Transfer Tokens**: Users can transfer tokens to another address.

## License

This contract is licensed under the MIT License. See the LICENSE file for more details.

## Author

Avinash 

avinashreddy777890@gmail.com
