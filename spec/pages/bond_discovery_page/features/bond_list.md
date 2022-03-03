# Bond list

## Purpose

The purpose of the bond list is to allow a user to discover bonds.

## Implementation

Lists will be implemented as a table.

### Headers

#### **Issuer**

- Description: This is the issuer of the bond
- Value: image and name of org
  - Ex: 🦄 Uniswap

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
