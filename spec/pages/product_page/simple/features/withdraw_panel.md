# Withdraw panel

## Purpose

The purpose of the withdraw panel is to allow users to withdraw funds after the maturity date.

## States

- Before maturity
  - Empty state
- After maturity
  - No default
    - Users can withdraw principle + interest in borrowed asset after maturity
  - Default
    - Users can withdraw any payments made in borrowed asset and collateral after maturity

## Implementation

The withdraw panel will be implemented as a panel.

### Withdraw panel

#### Information

- Simple status
  - Repaid
  - Partially repaid
  - Defaulted
- Balance
  - Description: Amount of Simple tokens in connected wallet
  - Value: number
    - Ex: 750,000 UNISWAP SIMPLE 07AUG2022 (USDC)
- Withdraw amount
  - Description: Amount of borrowed asset and collateral available to withdraw
  - Value: amount and type of assets
    - Ex: 500,640 USDC and 35 UNI

#### Inputs

- Withdraw button

## Examples

### Uniswap

![](../../../assets/uniswap/convert.png)
