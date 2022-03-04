# Auction config

## Purpose

The purpose of the auction config step is to allow the user to supply all the auction config details.

## Implementation

Auction config is a step in the auction creation page which contains sub-steps.

## Sub steps

### Schedule

**inputs**

- Start date

**display**

- End date (this was already chosen in bond config)
- Auction duration

### Bidding

**inputs**

- Minimum bid size
- Last date to cancel bid (must be in between start/end date)

**display**

### Type

**inputs**

- Type (private/public)
- if private
  - Signer address (this may not be needed, we can use the auction creator address as the signer)

**display**

- Link to docs explaining how signer works (explain the auction creator address is the signer)
- Tooltip saying addresses can be added to whitelist later
- Tooltip saying not to use an address with assets in it (need clarity on this)

### Information

**inputs**

- Issuer
- Auction description
- Prospectus link

**display**

- Link to docs explaining what a prospectus is
- Platform fee

### Review

**display**

- Start and end
  - Start date
  - End date
  - Duration
- Bidding
  - Minimum bid size
  - Last date to cancel bid (must be in between start/end date)
- Auction type
  - Type
  - if private
    - Signer address
- Auction information
  - Issuer
  - Auction description
  - Prospectus link
  - Platform fee

## Examples

### Copper Launch

Contract information

![](../../../assets/copper/auction_config.png)

Auction config

![](../../../assets/copper/bond_config.png)

Review

![](../../../assets/copper/auction_summary.png)
