# Redeem panel

## Purpose

The purpose of the redeem panel is to allow users to redeem bonds for funds after the maturity date.

## States

- Before maturity
  - Disabled state
- After maturity
  - Active state

## Implementation

The redeem panel will be implemented as a panel.

### Active state

#### Information

- Status
  - Repaid
  - Partially repaid
  - Defaulted
- Balance
  - Description: Amount of bonds in connected wallet
  - Value: number
    - Ex: 100,000 UNI SIMPLE 22AUG2022 2P USDC
- Amount of assets to receive
  - Description: Amount of borrowed asset and collateral available for redemption
  - Value: amount and type of assets
    - States:
      - Repaid
        - Only show borrowed asset (USDC)
          - Ex: 100,000 USDC
      - Partially repaid
        - Show borrowed asset (USDC) and collateral asset (UNI)
          - Ex: 50,000 USDC and 25,000 UNI
      - Defaulted
        - Only show collateral asset (UNI)
          - Ex: 50,000 UNI

#### Inputs

- Max button
  - Increases "Amount of bonds to redeem" to "Balance"
- Amount of bonds to redeem
  - Description: Amount of bonds user redeems
  - Value: number
    - Ex: 100,000 UNI SIMPLE 22AUG2022 2P USDC
- Redeem button
  - Becomes a "Connect wallet" if wallet isn't connected

### Disabled state

I'm not sure how best to handle this.
Objectives:

- Show user there is a "redeem panel" and how it might work
- Show user how many bonds they have in their wallet
- Explain to user when the panel will be active
  - Panel will be active at maturity date or when bond is repaid fully. Whichever comes first.
- Offer to notify the user when they use the panel

## Examples

### Uniswap

![](../../../../assets/uniswap/convert.png)
