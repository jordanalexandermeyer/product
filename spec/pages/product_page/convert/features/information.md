# Convert information

## Purpose

The purpose of Convert information is to display to the user necessary information regarding the bond.

## Implementation

The Convert information will be displayed in multiple panels.

### Panel 1: Convert Details

#### Type

- Description: Product type
- Value: enum + logo
  - ⏩ Convert

#### Name and address

- Description: The logo and name of the Convert token. Next to the name should be a link to the contract on etherscan
- Value: product name
  - Ex:
    - UNI CONVERT 24AUG2022 2P 25C USDC

#### Supply

- Description: This is the amount of bonds issued
- Value: amount
  - Ex: 50,000,000

#### Maturity date

- Description: Date the bond matures.
- Value: date
  - Ex: 24 AUG 2022 00:00 UTC

### Panel 2: Collateral

#### Collateral tokens

- Description: Type and amount of asset being provided as collateral per bond
- Value: numbers and types of asset
  - Ex: 0.5 UNI

#### Collateral token price

- Description: The current price of the asset provided as collateral in terms of the borrowed asset
- Value: numbers and types of asset
  - Ex: 10 USDC

#### Collateral value

- Description: The current value of the collateral in terms of the borrowed asset. This number comes from multiplying bond collateral by current token price
- Value: numbers and types of asset
  - Ex: 5 USDC

#### Put Strike price

- Description: Collateral token price at which the collateral token value equals the amount owed
- Value: number in borrowed asset
  - Ex: 2 USDC

### Panel 3: Convertibility

#### Convertible tokens

- Description: The amount of collateral asset each bond is convertible into
- Value: number and type of asset
  - Ex: 0.04 UNI

#### Convertible token price

- Description: The current price of the asset provided as collateral in terms of the borrowed asset
- Value: numbers and types of asset
  - Ex: 10 USDC

#### Convertible token value

- Description: Value of convertible tokens/bond.
- Value: number in borrowed asset
  - Ex: 0.4 USDC

#### Call Strike price

- Description: Collateral token price at which the convertible token value equals the amount owed
- Value: number in borrowed asset
  - Ex: 25 USDC

## Example

### Barnbridge

![](../../../../assets/barnbridge/bond_information.png)
![](../../../../assets/barnbridge/bond_information_large.png)
