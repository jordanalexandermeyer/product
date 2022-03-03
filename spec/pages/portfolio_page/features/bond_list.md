# Bond list

## Purpose

The purpose of the bond list is to allow a user to view their owned bonds and some important details about those bonds.

## Implementation

Lists will be implemented as a table. Each bond will link to its corresponding [bond page](../../bond_page/README.md).

### Headers

#### Issuer

- Description: This is the issuer of the bond
- Value: image and name of org
  - Ex: 🦄 Uniswap

#### **Amount**

- Description: How many bonds do I own?
- Value: number
  - Ex: 10,000,000

#### **Maturity date**

- Description: When does the bond mature?
- Value: date
  - Ex: 23 Aug 2022

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

### Barnbridge

![](../../../../../spec/assets/barnbridge/bond_list.png)
