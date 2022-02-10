# Handling default

## Implementation

### Part 1: Have debtors sign a loan agreement

#### Pros:

- Outlines the responsibilities of debtors
- Gives creditors some legal recourse, however limited

#### Cons:

- DAO members may not want to sign a legal document
- The legal enforceability is questionable

### Part 2: Pass off the handling of defaults to creditors and debtors

#### Pros:

- Allows us to scale better
- Having to arbitrate or manage defaults would be time consuming and we aren’t getting paid for it
- Reduces legal risk
- We may get sued if a creditor/debtor is unhappy with our arbitration
- Easier to implement
- Implementing smart contracts for arbitration would be a large lift

#### Cons:

- Reduces our skin in the game (bad for everyone but us)

### Part 3: Have a third party mediate/arbitrate the default

#### Pros:

- Gives a path forward for creditors and debtors
- Predetermined path forward so they won’t have to decide/argue about this later
- Creates a partnership for us
- That partner who does the mediation/arbitration will want us to succeed

#### Cons:

- Parties may not trust the third party
- If parties to the bond don’t trust the mediator/arbitrator, they may not issue a bond
- In the case of arbitration, the third party’s decision may not be enforceable
- Arbitration is usually legally binding. Without a legal system to enforce arbitration, the value is questionable

### Part 4: Defaults on multiple bonds

If a default occurs on one bond, it pushes all the bonds issued into default.

## User flow:

1. Loan agreement is signed by DAO core members prior to issuing bond
2. Bond is defaulted on
3. Value of collateral is transferred to bond holders
4. DAO and creditors undergo mediation using an agreed upon third party
   a. If a resolution is agreed on, it is implemented
   b. If not, the default moves to arbitration
5. DAO and creditors undergo arbitration using an agreed upon third party
   a. Whatever the arbitrator decides is implemented
6. If the arbiter decision is not implemented, bond holders can use loan agreement to take legal actions
