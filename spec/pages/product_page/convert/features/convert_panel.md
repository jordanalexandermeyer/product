# Redeem panel

## Purpose

The purpose of the actions panel is to allow users to redeem their Converts for convertible tokens before maturity.

## States

- Before maturity
  - Users can redeem bonds for portion of collateral
- After maturity
  - Panel is disabled

## Implementation

The redeem panel will have a different implementation and purpose depending on the state of the auction.

### Before maturity

#### Information

- Balance
  - Description: Amount of bonds in connected wallet
  - Value: number
    - Ex: 750,000 UNISWAP CONVERT 07AUG2022 USDC
- Conversion ratio
  - Description: Amount of collateral each bond is convertible to
  - Value: amount and type of asset
    - Ex: 0.5 UNI
- Conversion amount
  - Description: Amount of convertible tokens the entered amount of bonds can be convertible to. Calculate this and display it after a user has entered the "amount" input.
  - Value: amount and type of asset
    - Ex: 532 UNI
    - Add a parantheses with value in borrow token (USDC in this case)

#### Inputs

- Amount
  - Description: amount of bonds to convert to collateral asset
  - Value: amount and type of asset
    - Ex: 750,000 UNISWAP CONVERT 07AUG2022 USDC
- Convert button

### After maturity

- Empty state explaining bonds can no longer be converted

## Examples

### Uniswap

![](../../../../assets/uniswap/convert.png)
