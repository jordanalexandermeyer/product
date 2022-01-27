# Create auction page

## Purpose

The purpose of the create auction page is to allow the user to enter the necessary inputs for an auction and start it.

## Implementation

The page is implemented as a wizard with a main panel and sidebar displaying where the user is in the creation flow. Some steps have substeps that need to be completed to finish the main step. These steps should be displayed in a sidebar with substeps below them.

## Users

* Issuer
  * Auction creator/manager

## User flows

* [Start auction](../../user\_flows/start\_auction.md)

## User needs

| User   | User Wants                                                 | Product Needs                     |
| ------ | ---------------------------------------------------------- | --------------------------------- |
| Issuer | Wants to determine what the steps are to create an auction | Needs wizard to communicate steps |
|        | Wants to completely understand the data they are entering  | Needs tooltips to clarify inputs  |

## Stages

These are the stages of the wizard.

1. [Bond config](features/bond\_config.md)
   1. [Bond](features/bond\_config.md###bond)
   2. [Collateral](features/bond\_config.md###collateral)
   3. [Convertible](features/bond\_config.md###convertibility)
   4. [Review](features/bond\_config.md###review)
2. [Auction config](features/auction\_config.md)
   1. [Schedule](features/auction\_config.md###schedule)
   2. [Bidding](features/auction\_config.md###bidding)
   3. [Auction type](features/auction\_config.md###type)
   4. [Auction information](features/auction\_config.md###information)
   5. [Review](features/auction\_config.md###review)
3. [Review summary](features/review\_summary.md)
4. [Create auction](features/create\_auction.md)

## Examples

### Copper Launch

![](../../../../spec/assets/copper/auction\_creation\_page.png)
