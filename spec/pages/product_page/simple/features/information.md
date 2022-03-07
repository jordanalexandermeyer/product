# Simple information

## Purpose

The purpose of Convert information is to display to the user necessary information regarding the bond.

## Implementation

The Convert information will be displayed in a panel.

### Information to display

#### Type

- Description: Product type
- Value: enum + logo
  - 🟧 Simple

#### Name and address

- Description: The logo and name of the Simple token. Next to the name should be a link to the contract on etherscan
- Value: 🦄 Uniswap Simple

#### Supply

- Description: This is the amount of bonds issued
- Value: amount
  - Ex: 50,000,000

#### Maturity date

- Description: Date the bond matures.
- Value: date
  - Ex: Jan 19, 2023

#### Collateral

- Description: Type and amount of assets being provided as collateral for issuance. Most often there will only be one type, but we will support multiple types.
- Value: numbers and types of asset
  - Ex: 500,000 UNI, 200,000 RPL, 724,000 BAYC

#### Current token prices

- Description: The current prices of the assets provided as collateral in terms of the borrowed asset
- Value: numbers and types of asset
  - Ex: UNI 25.93 USDC, RPL 12.32 USDC, BAYC 1.02 USDC

#### Collateral value

- Description: The current value of the collateral in terms of the borrowed asset. These numbers come from multiplying bond collateral by current token prices
- Value: numbers and types of asset
  - 12,500,000 USDC, RPL 2,500,000 USDC, BAYC 750,000 USDC

#### Collateralization ratio

- Description: Calculated by dividing value of collateral offered by bonds issued.
- Value: percent
  - Ex: 350%

## Example

### Barnbridge

![](../../../assets/barnbridge/bond_information_large.png) ![](../../../assets/barnbridge/bond_information.png)
