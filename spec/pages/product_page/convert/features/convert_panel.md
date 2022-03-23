# Redeem panel

## Purpose

The purpose of the actions panel is to allow users to redeem their Converts for convertible tokens before maturity.

## States

- Before maturity
  - Active state
- After maturity
  - Disabled state

## Implementation

The redeem panel will have a different implementation and purpose depending on the state of the auction.

### Active state

#### Information

- Status
  - Active
    - Should indicate that this won't last forever
    - Ideas:
      - Active until 07AUG2022
      - Active until maturity
      - Active for 300 days 0 hours
- Balance
  - Description: Amount of bonds in connected wallet
  - Value: number
    - Ex: 100,000 UNI CONVERT 22AUG2022 2P 25C USDC
- Amount of assets to receive
  - Description: Amount of convertible tokens available for redemption
  - Value: amount and type of asset
    - Ex: 4,000 UNI

#### Inputs

- Max button
  - Increases "Amount of bonds to convert" to "Balance"
- Amount of bonds to convert
  - Description: amount of bonds to convert to collateral asset
  - Value: amount and type of asset
    - Ex: 100,000 UNI CONVERT 07AUG2022 2P 25C USDC
- Convert button
  - Becomes a "Connect wallet" if wallet isn't connected

### Disabled state

I'm not sure how best to handle this.
Objectives:

- Show user there was a "convert panel"
- Explain to user that conversions are no longer allowed after maturity date

## Examples

### Uniswap

![](../../../../assets/uniswap/convert.png)
