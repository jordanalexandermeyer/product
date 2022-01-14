# Individual auction page during auction

## State: During Auction

## Users

- Potential auction participant
- Auction creator/manager

## User assumptions

### Potential auction participant

- Knows how the auction works
  - User came to this page through landing page which has links to educational content
  - If they don't know how it works, they can learn via the link in the navbar

## User needs

### Potential auction participant

| User Wants                                                          | Product Needs                                                                 |
| ------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| Wants to determine whether they want to participate in this auction | Needs information regarding the bond auction                                  |
| Wants to determine current status of the auction                    | Needs to show current orders, current pricing, etc                            |
| Wants to participate in the bond auction                            | Needs to allow orders to be placed and cancelled                              |
| Wants to understand if order will be filled or not                  | Needs to display status of user's orders and whether or not it will be filled |

### Auction creator/manager

| Wants                        | Needs                                           |
| ---------------------------- | ----------------------------------------------- |
| Wants to view auction status | Needs to see current volume, pricing, bids, etc |
| Wants to manage the auction  | Needs a management section                      |

## Inspirations

- [Gnosis Auction](assets/gnosis/auction_page_during.png)
- [Copper Launch](assets/copper/auction_page_during.png)

## Features

### Warning

Explains to users the potential risk of participating in the auction.

- [Example](assets/copper/warning.png)

### Auction information

- Issuer name
  - Ex: Uniswap
- Auction status
  - Ex: Active
- Auction duration
  - Ex: 7 days
- Days/time until auction ends
  - Ex: 3 days, 3 hours
- Bond offering size
  - Ex: \$50M
- Total bid volume
  - Ex: \$30M
- Minimum funding threshold
  - Ex: \$30M
- Auction description
  - Abridged version of prospectus to give the reader a brief overview of who the issuer is and why they are issuing a bond
- Link to prospectus
  - Detailed document outlining all aspects of the bond offering
  - Ex: [Prospectus](https://www.sec.gov/Archives/edgar/data/320193/000119312513184506/d527270d424b2.htm)
- Maximum bond interest rate
  - The auction determines interest rate based on supply and demand. This is the maximum interest rate the issuer is willing to pay.
  - Ex: 15%
- Current auction interest rate
  - Ex: 8.5%
- Bond Term length
  - Ex: 12 months
- Bond Collateral stats
  - Type and amount
    - Ex: 500,000 UNI
  - Token contract address
  - Current collateralization ratio
- Convertibility
  - Are the bonds redeemable for a pro-rata portion of the collateral tokens?
  - Yes/No
  - Breakeven token price of convertibility
    - Ex: \$75
  - Current token price
    - Ex: \$25
  - Projected returns graph
    - [Example](assets/convertible_bond_graph.png)
      - This will be replaced by a better example

### Bid submission

- This is where users submit bids
- Accepts
  - Interest rate and volume
    - Ex: 5% and \$1,000,000
    - Interest rate is above 0
  - OR
  - Price and volume
    - Ex: 0.92 and \$1,000,000
    - Price will be between 0 and 1
- Examples
  - [Copper](assets/copper/bidding_during.png)
  - [Gnosis](assets/gnosis/bidding_during.png)

### Orderbook

- This is where bids are displayed
  - Bids should have the following info
    - Wallet address
    - Interest rate
    - Price
    - Volume
  - Should be sortable by Price, interest rate, or volume
- Examples
  - [Copper](assets/copper/order_book.png)
  - [Gnosis](assets/gnosis/order_book.png)

### Your orders

- This is where a users bids will be displayed once auction a user has placed a bid
  - Bids should have the following info
    - Wallet address
    - Interest rate
    - Price
    - Volume
    - Status
      - Ex: Cancelled/Active
    - Will order be filled?
      - Explanation: if order price is too low, it may not get filled
      - Yes/No
        - If yes, should be green, happy state indicator
        - If no, should have red, unhappy state indicator
  - Bids should be able to be cancelled
- Examples
  - [Copper](assets/copper/order_book.png)
  - [Gnosis](assets/gnosis/my_orders_empty.png)

### Graph

- This is a visual representation of all bids
- Tells user current state of the auction/pricing at a glance
- Examples
  - [Copper](assets/copper/order_book_graph.png)
  - [Gnosis](assets/gnosis/order_book_graph.png)

### Auction management

- Examples
  - [Copper](assets/copper/auction_management.png)