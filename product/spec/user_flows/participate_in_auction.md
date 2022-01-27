# Submits an order

## Inspiration

* [Copper Launch](https://docs.alchemist.wtf/copper/auction-participation-walkthrough)
* [Gnosis Auction](https://gnosis-auction.eth.link/#/start)
  * Go to docs
  * Click "Participate as a bidder"

## User flow

1. User starts on an auction page with an "Active" status

![](../../../spec/assets/copper/auction\_page.png)

2\. User sees warning outlining the dangers of participating in bond auctions

![](../../../spec/assets/copper/warning.png)

3\. User sees auction details

![](../../../spec/assets/copper/auction\_details.png)

![](../../../spec/assets/gnosis/auction\_details.png)

4\. User sees chart representing order book

![](../../../spec/assets/gnosis/order\_book\_graph.png)

5\. User sees bond details

![](../../../spec/assets/copper/bond\_details.png)

6\. User sees submit bid panel

![](../../../spec/assets/gnosis/place\_order.png)

7\. User approves the use of the bidding token

![](../../../spec/assets/gnosis/bidding\_during.png)

8\. User submits a bid by entering volume and interest rate (or price)

9\. A modal appears which shows bid transactions

![](../../../spec/assets/gnosis/place\_order\_confirm.png)

10\. User confirms a transaction to send funds and submit the bid

11\. Loading spinner appears until transactions are complete

![](../../../spec/assets/gnosis/place\_order\_loading.png)

12\. Happy state is shown once transactions are complete

13\. Bid shows up in "your orders" section

![](../../../spec/assets/gnosis/your\_order.png)

## Figma diagram

![](../../../spec/assets/porter/participate\_in\_auction\_user\_flow.png)
