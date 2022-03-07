# Product list

## Purpose

The purpose of the product list is to allow a user to discover products.

## Implementation

Lists will be implemented as a table.

### Headers

#### **Name**

- Description: This is the name of the bond
- Value: image and name of bond
  - Ex: 🦄 Uniswap Convert

#### **Supply**

- Description: This is the amount of bonds issued
- Value: amount
  - Ex: 50,000,000

#### **Maturity date**

- Description: Bond maturity date
- Value: date time
  - Ex: 23 AUG 2022

#### **Status**

- Description: What status is the bond?
- Value: enum
  - Active
  - Matured

#### **Type**

- Description: Product type
- Value: enum + logo
  - ↔️ Convert
  - 🟧 Simple
  - ♻️ Refi

## Examples

### Copper Launch

#### Auction panel

![](../../../../../spec/assets/copper/auction_discovery.png)

#### Vetted list

![](../../../../../spec/assets/copper/vetted_auction_list.png)

#### Unvetted list

![](../../../../../spec/assets/copper/unvetted_auction_list.png)
