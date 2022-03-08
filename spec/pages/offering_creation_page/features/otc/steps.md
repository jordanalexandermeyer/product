# OTC steps

## Purpose

The purpose of the OTC steps is to allow the user to supply all the offering config details.

## Implementation

Multiple sub steps are listed here that can be used in different offering wizards.

Sub steps are shown in the wizard
![](../../../assets/balancer/wizard_steps.png)

## Sub steps

### Product

**inputs**

- Product for sale
  - If they have a product they've created with Porter, show this as an option
- Amount of product they want to sell
  - They may have minted 5,000,000 tokens with Convert but only want to sell 4,000,000
  - Allow them to enter amount they want to sell

**display**

- Display link to product page
- Display amount of product tokens they have

### Schedule

**inputs**

- Start date (locked to today because auction starts as soon as it's created)
- End date

**display**

- Length of offering

### Order

**inputs**

- Price/Interest rate
  - Price can be converted to interest rate
- Minimum order size
  - Minimum amount of tokens that can be used for an order
- Access
  - Public
  - Private
    - If private
      - Signer address

### Confirm creation

**inputs**

- Create button
  - ![](../../../assets/balancer/approve_steps.png)
- Description
  - Allows user to write a paragraph about the offering

**display**

- Summary
  - Product
  - Offering type
    - OTC
  - Amount for sale
  - Start & End date
  - Price/Interest rate
  - Minimum order size
  - Public/Private
