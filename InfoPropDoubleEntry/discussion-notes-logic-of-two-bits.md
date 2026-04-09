# Discussion Notes: The Logic of the Two-Bit Result

**Date:** April 7, 2026
**Participants:** Rick Antle, Claude

## Starting question

What drives the paper's result? Can we see it without vectors and matrices, in terms of how actual accounting systems work?

## The interest rate swap as a running example

An interest rate swap currently sits as an asset on the balance sheet. What can happen to it?

1. **Nothing changes.** The interest rate stays the same, the swap remains an asset.
2. **The rate moves against you to zero.** Neither party owes the other. The swap asset disappears, a loss is recognized on the income statement. No cash changes hands.
3. **The rate moves against you further.** The swap flips from asset to liability. A larger loss is recognized. No cash changes hands.
4. **The rate moves in your favor.** The swap increases in value, a gain is recognized. No cash changes hands.
5. **The swap is settled for cash.** The contract matures, cash comes in, the asset disappears from the balance sheet.

## The redundancy problem

For events 2–4 (revaluations, no cash), the income statement and cash flow statement appear to be redundant. The loss or gain hits the income statement, and the cash flow statement simply adds it back as a non-cash item. If you know what happened on the income statement, you already know what the cash flow statement will say. This seems like one bit expressed three times, not two bits.

## The breakthrough: settlement vs. revaluation

Focus on just two events — settlement (event 5) and revaluation to zero (event 2). In both cases the swap asset disappears from the balance sheet. But:

- **Settlement (case 1):** Cash goes up, equity is unchanged. No gain or loss on the income statement. The cash flow statement shows a real cash inflow.
- **Revaluation to zero (case 2):** Cash is unchanged, equity drops (the loss reduces retained earnings). The income statement shows a loss. The cash flow statement adds it back.

If you show cash explicitly on the balance sheet: in case 1, the swap disappears and cash goes up. In case 2, the swap disappears and equity goes down. The balance sheet *alone* can distinguish these — but only because you can see both cash and equity, not just the swap.

## The two independent dimensions

When something happens to a non-cash asset, there are two independent questions:

1. **Did cash change?** (The cash dimension)
2. **Did equity change?** (The equity dimension)

These are genuinely independent. The four possible combinations are:

| Cash changed? | Equity changed? | Example |
|---|---|---|
| No | No | Nothing happens |
| No | Yes | Swap revalued to zero (loss, no cash) |
| Yes | No | Swap settled at carrying value (cash, no gain/loss) |
| Yes | Yes | Swap settled at a different value (cash + gain/loss) |

Four combinations = two bits.

The balance sheet identity (Assets = Cash + Equity, simplified) means that any change in a non-cash asset must show up as a change in cash, a change in equity, or both. There are exactly two degrees of freedom. The accounting identity and the cash flow reconciliation identity together keep those two dimensions separately visible across the financial statements.

## Potential significance for the paper

This may provide a much more accessible way to explain the paper's result than the vector/matrix formalism. The two-bit capacity arises because the double-entry system with articulating statements tracks two independent economic dimensions — the cash effect and the equity effect — for every account. The multi-statement architecture is what keeps those dimensions separately observable.

## Open questions

- Does this interpretation map cleanly onto the paper's formal structure? Specifically, do "did cash change" and "did equity change" correspond to the two rows of the paper's column vectors?
- The paper's result requires a second account even though it doesn't change. What role does the second account play in this interpretation?
- Does this interpretation help explain why the paper abstracts away magnitudes? (Perhaps the two-bit result is about the existence of two independent dimensions, not their magnitude.)
- How does this connect to the paper's X and Z operators? X (reclassification) seems to be about moving between the equity dimension and the cash dimension. Z (revaluation) is about the equity dimension only.

## Notation discussion

The paper uses A and E for both the accrual-statement row and the cash-flow-statement row, which is confusing because they mean different things on each row. Rick proposed: A (asset) and E (expense) for the accrual statement, O (operations) and I (investing) for the cash flow statement. This makes the articulation constraint transparent: A pairs with I, E pairs with O.
