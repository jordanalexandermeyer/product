# Bond config

## Purpose

The purpose of the bond config step is to allow the user to supply all the bond config details.

## Implementation

Bond config is a step in the auction creation page which contains sub-steps.

## Sub steps

### Bond

**inputs**

- Borrow token contract address
- Max annual interest rate
- Bond issuance date (this will be the auction end date)
- Bond maturity date
- Maximum issuance size
- Minimum issuance size

**display**

- Borrow token logo
- Borrow token name
- Borrow token ticker
- Term length (years)
- Max interest owed at maximum issuance
- Max interest owed at minimum issuance

### Collateral

**inputs**

- Collateral (yes/no)
  - if yes
    - Collateral token contract address
    - Collateral token amount/ratio (can switch between)

**display**

- Link to docs explaining how collateral works
- if collateral
  - Collateral token logo
  - Collateral token name
  - Collateral token ticker
  - Collateral token balance
  - Collateral token price (in terms of borrow token)
  - Current value of collateral (in terms of borrow token)

### Convertibility

If there is no collateral, the bond cannot be convertible. Display a message explaining this and disable inputs if there is no collateral.

**inputs**

- Convertible (yes/no)
  - if yes
    - Convertible token amount (must be lower than or equal to bond collateral token amount)

**display**

- Link to docs explaining how convertibility works
- if convertible
  - Breakeven token price of convertibility (in terms of borrow token)
  - Link to docs explaining breakeven token price

### Review

**display**

- Bond
  - Borrow token contract address
  - Borrow token logo
  - Borrow token name
  - Borrow token ticker
  - Max annual interest rate
  - Bond issuance date
  - Bond maturity date
  - Term length
  - Maximum issuance size
  - Minimum issuance size
  - Maximum interest owed at maximum issuance size (optional)
  - Maximum interest owed at minimum issuance size (optional)
- Collateral
  - if yes
    - Collateral token contract address
    - Collateral token logo
    - Collateral token name
    - Collateral token ticker
    - Collateral token amount
    - Collateral token ratio
    - Collateral token price (in terms of borrow token)
    - Current value of collateral (in terms of borrow token)
  - if no
    - None
- Convertible
  - if yes
    - Convertible token amount
    - Breakeven token price of convertibility (in terms of borrow token)
  - if no
    - No

## Examples

### Copper Launch

Contract information

![](../../../assets/copper/token_information.png)

Review

![](../../../assets/copper/auction_summary.png)
