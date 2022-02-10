# Bond list

## Purpose

The purpose of the bond list is to allow a user to view their owned bonds and some important details about those bonds.

## Implementation

Lists will be implemented as a table. Each bond will link to its corresponding [bond page](../../bond_page/README.md).

### Headers

#### Bond name

- Description: The name of the bond token
- Value: UNISWAP CONVERT (UNI) 07AUG2022 (USDC)

#### **Amount**

- Description: How many bonds do I own?
- Value: number
  - Ex: 10,000,000

#### **Value of convertible asset (if convertible)**

- Description: The value of the convertible asset
- Value: 6,000,000 USDC
  - Ex: 6,000,000 USDC

#### **Status**

- Description: What status is the bond?
- Value: enum
  - Outstanding
  - Matured
  - In default

## Examples

### Barnbridge

![](../../../../../spec/assets/barnbridge/bond_list.png)
