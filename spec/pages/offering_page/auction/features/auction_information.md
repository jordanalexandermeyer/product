# Auction information

## Purpose

The purpose of auction information is to display to the user necessary information regarding the current state of the auction. Some information displayed will change depending on the current state of the auction while others will always be displayed.

## States

- Active
  - Auction is ongoing
- Ended
  - Auction has ended

## Implementation

The auction information will be displayed at the top of the page in a grid.

### Information to display

#### **Issuer**

- Description: This is the creator of the auction and issuer of debt
- Value: image and name of org
  - Ex: 🦄 Uniswap

#### Status

- Description: The current status of the auction
- Value: Depends on auction state
  - Examples:
    - Active
    - Ended

#### Start date

- Description: start time of auction
- Value: datetime
  - Ex: 2022-02-08 13:00 UTC

#### End date

- Description: end time of auction
- Value: datetime
  - Ex: 2022-02-08 13:00 UTC

#### **Offering size**

- Description: This is the amount of bonds the issuer is selling
- Value: amount
  - Ex: 50,000,000

#### Total bid volume

- Description: Sum of all bids submitted in auction
- Value: amount and type of asset
  - Ex: 75,000,000 USDC

#### Minimum funding threshold

- Description: Bid volume required for auction to settle
- Value: amount and type of asset
- Ex: 30,000,000 USDC

#### Minimum bid size

- Description: Bid size required to participate
- Value: amount and type of asset
- Ex: 1,000 USDC

#### Current auction interest rate (Active only)

- Description: The interest rate that would be set if the auction were to end with no more bids being submitted.
- Value: percent
  - Ex: 8%

#### Clearing auction interest rate (Ended only)

- Description: The interest rate that was set for the auction.
- Value: percent
  - Ex: 8%

#### Maximum interest rate

- Description: The auction determines interest rate based on supply and demand. This is the maximum interest rate the issuer is willing to pay.
- Value: percent
  - Ex: 15%

## Examples

### Gnosis Auction

![](../../../../../spec/assets/gnosis/auction_details.png)

### Copper Launch

![](../../../../../spec/assets/copper/auction_details.png)
