# Feature Roadmap, Module 4 · BU Pay & Credit

**Scenario:** Riverty BU Pay & Credit, First Consumer Card

**Team:** [your assumed team size]

## Strategic anchors
- **Persona:** An existing Riverty BNPL user with an activated card who uses it for small everyday purchases in store and wants to pay later wherever they shop (N-01, N-04).
- **Primary metric:** In-store decline rate: 8.7% in Month 4 (7.9% across the pilot, 48 of 604 attempts), with a target below 4%.
- **Moment of misery:** Declined at the till with no reason shown, so they go back to their debit card (N-06, T-101).
- **Guardrail:** On-time repayment rate of card holders. Cutting declines must not raise missed payments. The baseline still has to come from Risk.

## Scoring
| Feature | Value | Effort | Quadrant | Decision | Rationale |
|---|---|---|---|---|---|
| B1 Decline reason and retry hint shown in the app | 4 | 2 | Quick Win | Now | It tackles the moment of misery head on (N-06, T-101) and gives us the decline reasons we need to target the fix. |
| B2 Add to phone wallet straight from the approval screen | 3 | 2 | Fill-In | Later | It is cheap, and a third of activated cards never reach the wallet (T-102), so in-store use stays blocked without it. |
| B3 One balance view for card and regular pay later orders | 2 | 4 | Time Sinker | Cut | The pain is real (T-103, N-07), but it comes after the till and touches the ledger. |
| B4 Choose pay now or pay later per purchase after paying | 2 | 4 | Time Sinker | Cut | It doesn’t help at the till, and changing repayment after purchase puts the repayment guardrail at risk. |
| B5 Offers from partner merchants inside the card app | 1 | 3 | Time Sinker | Cut | It is a Sales ask that does nothing for a card declined at a bakery. |
| B6 Fix in-store declines at pharmacy, fuel and grocery terminals with the processor | 5 | 3 | Major Project | Next | It is the only feature that lowers the decline rate itself (8.8% to 8.9% in these categories), guided by B1’s reason codes and without loosening risk rules. |
| B7 Physical card | 3 | 5 | Time Sinker | Cut | It helps people without a phone wallet pay in store, but issuing takes months. Revisit if B2 doesn’t close the wallet gap. |
| B8 One due date for card and pay later orders | 2 | 5 | Time Sinker | Cut | It fixes the two due dates (T-104), but nothing at the till, and it likely needs a credit policy change (N-11). |

## Roadmap
### NOW, this sprint
- **B1 Decline reason and retry hint shown in the app**, It tackles the moment of misery head on (N-06, T-101) and gives us the decline reasons we need to target the fix.

### NEXT, the following sprints
- **B6 Fix in-store declines at pharmacy, fuel and grocery terminals with the processor**, It is the only feature that lowers the decline rate itself (8.8% to 8.9% in these categories), guided by B1’s reason codes and without loosening risk rules.

### LATER, backlog
- **B2 Add to phone wallet straight from the approval screen**, It is cheap, and a third of activated cards never reach the wallet (T-102), so in-store use stays blocked without it.

### ✂ Cut List
- **B3 One balance view for card and regular pay later orders**, The pain is real (T-103, N-07), but it comes after the till and touches the ledger.
- **B4 Choose pay now or pay later per purchase after paying**, It doesn’t help at the till, and changing repayment after purchase puts the repayment guardrail at risk.
- **B5 Offers from partner merchants inside the card app**, It is a Sales ask that does nothing for a card declined at a bakery.
- **B7 Physical card**, It helps people without a phone wallet pay in store, but issuing takes months. Revisit if B2 doesn’t close the wallet gap.
- **B8 One due date for card and pay later orders**, It fixes the two due dates (T-104), but nothing at the till, and it likely needs a credit policy change (N-11).
