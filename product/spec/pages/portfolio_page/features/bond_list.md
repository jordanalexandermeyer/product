# Bond list

## Purpose

The purpose of the bond list is to allow a user to view their owned bonds and some important details about those bonds.

## Implementation

Lists will be implemented as a table.

### Headers

#### **Issuer**

* Description: This is the issuer of debt
* Value: image and name of org
  * Ex: 🦄 Uniswap

#### **Term length**

* Description: The time from issuance to maturity date
* Value: months
  * Ex: 12 months

#### **Maturity date**

* Description: The date the bond can be exchanged for interest + principle
* Value: date
  * Ex: Jan 18, 2023

#### **Interest rate**

* Description: The fixed interest rate set at issuance
* Value: percent
  * Ex: 15%

#### **Collateral % (maybe not)**

* Description: The value of the collateral divided by the bond value
* Value: percent and type of asset
  * Ex: 50% UNI

#### **Convertible %**

* Description: The value the convertible collateral divided by the bond value
* Value: percent and type of asset
  * Ex: 110% UNI

#### **Value**

* Description: The bond value assuming the bond linearly increases in value to par value
* Value: percent and type of asset
  * Ex: 110% UNI

#### **Amount**

* Description: How many bonds do I own?
* Value: number
  * Ex: 10,000,000

#### **Status**

* Description: What status is the bond?
* Value: enum
  * Active
  * Matured
  * Delinquent
  * In default

## Examples

### Barnbridge

![](../../../../../spec/assets/barnbridge/bond\_list.png)
