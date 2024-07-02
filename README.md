### IndoorGameToken 

#### Overview
The IndoorGameToken smart contract is designed to manage a tokenized system for an indoor game, allowing players to acquire game tokens of different levels (Beginner, Intermediate, Advanced) through token redemption. This contract extends ERC20 functionality to manage token creation, transfer, and burning, and integrates Ownable for ownership control.

#### Features
1. **Token Minting and Burning**
   - The contract owner can mint new tokens using `mintTokens`.
   - Players can burn their tokens using `burnTokens` after acquiring them.

2. **Token Redemption**
   - Players can redeem tokens for game levels (Beginner, Intermediate, Advanced) using `RedeeemGameToken`. Each level has a specific token cost which is deducted from the player's balance upon redemption.

3. **Ownership**
   - The contract owner has exclusive rights to mint tokens and can transfer ownership to another address.

4. **Events**
   - `GameTokenAcquired` event is emitted whenever a player successfully redeems tokens for a game level, capturing player address, game level, and token cost.

#### Token Costs
- `BeginnerTokenCost`: 500 tokens
- `IntermediateTokenCost`: 750 tokens
- `AdvancedTokenCost`: 1000 tokens

#### Requirements
- Solidity version ^0.8.18
- OpenZeppelin contracts for ERC20 token standard and access control (`Ownable.sol`).

#### Deployment
The contract `IndoorGameToken` requires an initial owner upon deployment, who has the exclusive right to mint tokens.

#### Usage
1. **Token Acquisition**
   - Players acquire tokens by calling `RedeeemGameToken` with the desired game level number (1 for Beginner, 2 for Intermediate, 3 for Advanced).

2. **Token Transfer**
   - Tokens can be transferred to other addresses using `transferGameTokens`.

3. **Ownership Management**
   - Ownership can be transferred using the `transferOwnership` function inherited from `Ownable`.
   - 
  ### License 
   - MIT License: Permission to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, with no warranty.
   - 
### Author 

Avinash

avinashreddy777890@gmail.com
