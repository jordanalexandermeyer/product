# Collateral liquidation

## Implementation

Allow issuers to liquidate themselves with flash loans

### Pros:

- Issuers can use collateral to repay loans early.
  - If the collateral has gone up in value and the issuer wants to use the collateral to repay the loan, they can take out a flash loan, swap it to Uniswap or another protocol, and pay off their bonds.
- No need for oracles.
  - If a default occurs and the collateral cannot be used to pay off the unpaid principal + interest, it must be less valuable than the unpaid principal + interest. Therefore, it is transferred to the bond holders.

### Cons:

- Using a flash loan is complex and will require the DAO to write custom smart contracts
  - We could write smart contracts for the DAO to use to liquidate themselves.
- It may be difficult to line up a large amount of liquidity for collateral sales.
  - However, that means it would have been difficult for bondholders to line up the liquidity as well.

## User flow:

1. For non-convertible bonds, we will allow DAOs to take out a flashloan from the collateral contract to repay the bond’s principal and interest
2. If the principal and interest is not repaid by the maturity date, bondholders will be able to redeem their bonds for the collateral and a defaulted bond token. This token represents the unpaid debt the DAO owes the bondholders.
