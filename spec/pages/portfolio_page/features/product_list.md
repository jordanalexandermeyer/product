# Product list

## Purpose

The purpose of the product list is to allow a user to view their owned products and some important details about those products.

## Implementation

Lists will be implemented as a table. Each product will link to its corresponding [product page](../../bond_page/README.md).

### Headers

#### Issuer

- Description: This is the issuer of the product
- Value: image and name of org
  - Ex: 🦄 Uniswap

#### **Type**

- Description: Product type
- Value: enum + logo
  - ↔️ Convert
  - 🟧 Simple
  - ♻️ Refi

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

## Examples

### Barnbridge

![](../../../../../spec/assets/barnbridge/bond_list.png)
