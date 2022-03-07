# Auction management

## Purpose

The purpose of auction management is to allow the auctioneer to manage the auction.

## States

- Active
  - Auction is ongoing
- Ended
  - Auction has ended

## Implementation

Should only be viewable by the creator of the auction.

### Functionality

#### Whitelist participants **(Active only)**

- Description: The list of participant wallet addresses that can participate in the auction.
- Value: options
  - CSV file
  - Comma separated list

#### Execute auction and claim funds **(Ended only)**

- Description: The auction creator can execute the auction after it has ended. This action is permissionless but it is the responsibility of the creator. Funds are automatically distributed to the auction creator's wallet.
- Value: button

## Examples

### Copper Launch

![](../../../assets/copper/auction_config.png)
