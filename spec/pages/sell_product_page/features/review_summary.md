# Review summary

## Purpose

The purpose of the review summary step is to allow the user to review all the data they've entered and confirm everything is correct.

## Implementation

Review summary is a step in the auction creation page which lists information about the bonds and auction.

**display**

* Bond config
  * Bond
    * Borrow token contract address
    * Borrow token logo
    * Borrow token name
    * Borrow token ticker
    * Max annual interest rate
    * Bond issuance date
    * Bond maturity date
    * Bond term length
    * Maximum issuance size
    * Minimum issuance size
    * Maximum interest owed for maximum issuance size
    * Maximum interest owed for minimum issuance size
  * Collateral
    * if yes
      * Collateral token contract address
      * Collateral token logo
      * Collateral token name
      * Collateral token ticker
      * Collateral token amount
      * Collateral token ratio
      * Collateral token price (in terms of borrow token)
      * Current value of collateral (in terms of borrow token)
    * if no
      * None
  * Convertible
    * if yes
      * Convertible token amount
      * Breakeven token price of convertibility (in terms of borrow asset)
    * if no
      * No
* Auction config
  * Start and end
    * Start date
    * End date
    * Duration
  * Bidding
    * Minimum bid size
    * Last date to cancel bid (must be in between start/end date)
  * Auction type
    * Type
    * if private
      * Signer address
  * Auction information
    * Issuer
    * Auction description
    * Prospectus link
    * Platform fee

## Examples

### Copper Launch

Contract information

![](../../../assets/copper/token\_information.png)

Auction config

![](../../../assets/copper/bond\_config.png)

Review

![](../../../assets/copper/auction\_summary.png)
