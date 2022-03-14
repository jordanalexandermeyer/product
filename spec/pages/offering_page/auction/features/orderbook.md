# Orderbook

## Purpose

The purpose of the orderbook is to display all the bids submitted during the auction.

## States

- Active
  - Auction is ongoing
- Ended
  - Auction has ended

## Implementation

The orderbook will be a table with headers at the top and each order represented by a row. Each column will be sortable.

There should be a second tab named "my orders" that allows the user to see their orders. [User orders](user_orders.md)

### Headers

#### Time

- Description: The time the bid was submitted
- Value: date and time
  - Ex: Jan 14, 2022, 12:00 UTC

#### Price

- Description: The bond price submitted as part of the bid.
- Value: amount and type of asset
  - Ex: 0.875 USDC

#### Interest rate

- Description: The interest rate submitted as part of the bid.
- Value: percent
  - Ex: 13%

#### Amount

- Description: The size of the bid
- Value: amount and type of asset
  - Ex: 750,000 USDC

#### Actions

- Description: Actions user can take
- Value: buttons
  - View transaction (etherscan link)

## Examples

### Gnosis Auction

![](../../../../assets/gnosis/order_book.png)

### Copper Launch

![](../../../../assets/copper/order_book.png)

### Balancer

![](../../../../assets/balancer/my_investments.png)
