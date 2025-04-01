# Daily-Check-In-Rewards
# Daily Login Reward Smart Contract

## Overview
This Solidity smart contract rewards users for logging in daily. Users can claim a fixed reward once every 24 hours, and their rewards are stored within the contract.

## Features
- Users can claim rewards once per day.
- Keeps track of the last claimed timestamp for each user.
- Rewards are stored in a balance mapping.
- No external imports or constructors for simplicity.

## Smart Contract Functions
### `claimReward()`
- Allows users to claim their daily reward.
- Ensures that at least 24 hours have passed since the last claim.
- Updates the user's balance upon successful claim.

### `getBalance()`
- Returns the total accumulated rewards of the caller.

## Deployment Instructions
1. Use a Solidity-compatible development environment (e.g., Remix, Hardhat).
2. Compile and deploy the contract.
3. Users can interact with the contract by calling `claimReward()` and checking their balance using `getBalance()`.

## Technical Details
- **Reward Amount:** `1 ether` (for representation, not actual ETH).
- **Claim Interval:** `1 day` (24 hours between claims).
- **Storage:** Uses mappings to track last claim times and balances.

## Notes
- This contract does not distribute real tokens but keeps an internal record of rewards.
- The values can be adjusted within the contract code before deployment.

## License
This project is open-source and available for modification and distribution under the MIT License.

