# Bond information

## Purpose

The purpose of bond information is to display to the user necessary information regarding the bond offering.

## Implementation

The bond information will be displayed toward the bottom of the page in a grid.

### Information to display

#### Bond name and address

- Description: The name of the bond token. Next to the name should be a link to the contract on etherscan
- Value: UNI CONVERT 07AUG2022 (USDC)

#### Supply

- Description: This is the amount of bonds issued
- Value: amount
  - Ex: 50,000,000

#### Type

- Description: Product type
- Value: enum + logo
  - ↔️ Convert
  - 🟧 Simple
  - ♻️ Refi

#### Maturity date

- Description: Bond maturity date
- Value: date time
  - Ex: 23 AUG 2022

#### Bond collateral

- Description: Type and amount of assets being provided as collateral for bond issuance.
- Value: numbers and types of asset
  - Ex: 500,000 UNI, 200,000 RPL, 724,000 BAYC

#### Current token prices

- Description: The current prices of the assets provided as collateral in terms of the borrowed asset
- Value: numbers and types of asset
  - Ex: UNI 25.93 USDC, RPL 12.32 USDC, BAYC 1.02 USDC

#### Bond collateral value

- Description: The current value of the collateral in terms of the borrowed asset. These numbers come from multiplying bond collateral by current token prices
- Value: numbers and types of asset
  - 12,500,000 USDC, RPL 2,500,000 USDC, BAYC 750,000 USDC

#### Current collateralization ratio

- Description: Calculated by dividing value of collateral offered by maturity value of bonds issued.
- Value: percent
  - Ex: 50%

#### Conversion ratio

- Description: The amount of collateral asset each bond is convertible into
- Value: numbers and types of asset
  - Ex: 0.01 UNI, 0.2 RPL, 0.3 BAYC

## Example

### Copper Launch

![](../../../assets/copper/bond_details.png)
