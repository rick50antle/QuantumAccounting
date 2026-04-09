# Continuation Doc: "An Information Property of Double Entry Accounting"

## Context

Rick Antle is working with coauthors John Fellingham, Haijin Lin, and Doug Schroeder on the paper "An Information Property of Double Entry Accounting" (March 2025). The paper models the double-entry accounting system as a communication channel using information theory (Shannon 1948). T-accounts are two-element vectors, journal entries are 2x2 matrices (X = reclassification, Z = revaluation), and the central result is that one account can transmit two bits of information when two articulating financial statements and at least two accounts satisfy the accounting identity and cash flow reconciliation identity.

## Files in this folder

- `Info-Property-Double-Entry-202503.docx` — the paper (original Word document)
- `Info-Property-Double-Entry.md` — the paper converted to markdown
- `memo-structure-and-magnitudes.pdf` — revised memo from Rick to coauthors (April 4, 2026), sent to coauthors
- `memo-structure-and-magnitudes.md` — markdown source of the memo
- `discussion-notes-structure-and-magnitudes.md` — earlier draft essay (superseded by the memo)

## What we discussed (two sessions)

### Session 1 (prior): Modeling foundations

Extended conversation about the vector representation of accounts and the decision to abstract away from magnitudes. Key conclusions:

1. **Abstracting magnitudes is reasonable** — isolates the structural contribution; the two-bit result is a floor on capacity, not a ceiling.
2. **Asset vs liability is a magnitude distinction** — a "negative asset" is a liability (interest rate swaps illustrate this). Every within-statement distinction is a magnitude distinction.
3. **The irreducible structural distinction is resources vs claims** — the accounting identity A = E separates resources from claims. These are not positive and negative versions of the same quantity.
4. **A = E alone is nearly trivial — articulation is what matters** — two simultaneous constraints (accounting identity + cash flow reconciliation) create exploitable redundancy.
5. **The equity boundary is the dividing line** — structural capacity is engaged only when equities are affected. Asset swaps and liability settlements don't use the multi-statement architecture.
6. **The result is general across institutional settings** — for-profit, nonprofit, and governmental fund accounting all use the same architectural mechanism.

### Session 2 (current): Introduction reframing, the Z operator, and proofs

#### New introduction for the paper

Rick decided the paper should NOT lead with the for-profit example (risks being dismissed as well known). Instead, lead with the general architectural insight. Two proposed paragraphs were drafted and placed in the memo:

**Paragraph 1** opens with: double-entry systems share a common architectural feature — multiple articulating statements constrained to reconcile. Three institutional settings (for-profit, nonprofit, governmental fund accounting) are presented as coordinate examples of the same mechanism. Individual account balances convey magnitude information; the articulating architecture adds capacity beyond that.

**Paragraph 2** opens with: "This paper develops an algebra for analyzing the use of articulated statements to convey information." This frames the contribution as developing the algebra (not merely applying quantum mechanics). The algebra is the paper's contribution; the quantum information roots are background, not the point.

#### Fund accounting clarification

Rick initially questioned whether articulation expands capacity in fund accounting, since there is no breakdown of fund balance for a particular fund. Resolution: the decomposition that matters is not *of* fund balance but of the *change* in fund balance, which lives on the articulating operating statement (Statement of Revenues, Expenditures, and Changes in Fund Balance). This is the same mechanism as for-profit — retained earnings isn't decomposed on the balance sheet either; the income statement explains how it changed. GASB 54 categories (nonspendable, restricted, etc.) are about spending constraints, not sources of change, and are irrelevant to the paper's mechanism.

#### The Z operator and "revaluation"

Rick observed that "revaluation" is the wrong name if we're ignoring magnitudes, since revaluation in practice means changing a dollar amount. Discussion of what Z actually does: it flips an asset to a negative asset (A → Â) — a structural sign reversal within a statement. Applied to expenses/revenues, Z is the identity.

The write-down example in Section 4.2 smuggles magnitudes back in. A better example is an **interest rate swap** flipping from asset to liability: same contract, same account, structural sign flip, no magnitudes needed. Rick concluded that the swap example rescues the name "revaluation" — the contract's structural classification genuinely changes.

**Action item for the paper:** Replace the write-down illustration of Z in Section 4.2 with the interest rate swap example.

#### Interest in proofs and alternative proofs

Rick expressed particular interest in examining the proofs of the propositions and theorems, and in exploring whether alternative proofs exist. This was not yet discussed in detail. The key results to examine are:

- **Proposition 2** (Section III): Two-bit capacity requires each account to appear on both statements in structurally different roles (one A, one E per column). Only 4 of 16 configurations achieve this. Proof is in Appendix A (starts around line 835 in the markdown).
- **The Theorem** (Section IV): Generalizes Proposition 2 to n ≥ 2 accounts — one account can transmit two bits when at least two accounts satisfy both the accounting identity and the cash flow reconciliation identity. Proof is in Appendix A (starts around line 1039).
- **Observation 1** (Section II): Completeness of X and Z — any non-cash account can be reached from any other using combinations of X and Z, and all combinations reduce to {I, X, Z, XZ}.
- **Proposition 3** (Section IV): Restates Proposition 2 in accounting terms — the superposition and articulation properties together yield two-bit capacity with two accounts.

Questions Rick may want to explore:
- Are there more direct or intuitive proofs of Proposition 2 and the Theorem?
- Can the results be proved using purely algebraic or combinatorial arguments rather than exhaustive enumeration of configurations?
- Is there a cleaner way to establish the necessity direction (why the other 12 configurations fail)?
- Does the proof of the Theorem's generalization from 2 to n accounts have a more elegant form?
- Are the proofs as tight as they could be, or do they prove more than stated?

### Session 3: The economic logic of the two-bit result

Rick wanted to understand the paper's result without relying on the vector/matrix formalism — to find the economic substance behind the algebra.

#### The vector representation, clarified

An account vector captures structural classification only: which statement the account sits on and which side. E = [1 0] means income statement, A = [0 1] means balance sheet. Magnitudes are normalized away. The paper's column vectors represent pairs of classification decisions — one for the accrual statement, one for the cash flow statement — and articulation constrains which pairs are valid.

#### Notation confusion identified

The paper uses A and E for both rows of the column vector, even though they mean different things on each row. On the top row (accrual statement): A = asset on the balance sheet, E = expense on the income statement. On the bottom row (cash flow statement): A = no adjustment needed, E = adjustment required. Rick proposed better notation: A/E for the top row, O (operations) / I (investing) for the bottom row. This makes articulation constraints immediately readable: A pairs with I, E pairs with O.

#### The redundancy problem

For non-cash events (revaluations), the income statement and cash flow statement appear redundant. A loss hits the income statement, and the cash flow statement adds it back. One bit expressed three times, not two bits.

#### The breakthrough: two independent dimensions

Using the interest rate swap example, Rick identified two cases where the swap asset disappears from the balance sheet but for fundamentally different reasons:

- **Settlement:** Cash goes up, equity unchanged. The cash flow statement shows a real cash inflow.
- **Revaluation to zero:** Cash unchanged, equity drops. The income statement shows a loss, the cash flow statement adds it back.

**Key insight:** When something happens to a non-cash asset, there are two independent questions: (1) Did cash change? (2) Did equity change? These are genuinely independent, giving four combinations = two bits.

The balance sheet identity (Assets = Cash + Equity) means any change in a non-cash asset has exactly two degrees of freedom. The multi-statement architecture keeps those two dimensions separately visible.

#### Open questions from this session

- Does "did cash change" / "did equity change" map cleanly onto the paper's two-row column vectors?
- What role does the second account play in this economic interpretation?
- How do X and Z map onto cash vs. equity effects? X (reclassification) seems to involve both dimensions; Z (revaluation) seems to involve only equity.
- Can this economic interpretation be formalized as an alternative proof of the main results?

## Files in this folder

- `Info-Property-Double-Entry-202503.docx` — the paper (original Word document)
- `Info-Property-Double-Entry.md` — the paper converted to markdown
- `memo-structure-and-magnitudes.pdf` — revised memo from Rick to coauthors (April 4, 2026), sent to coauthors
- `memo-structure-and-magnitudes.md` — markdown source of the memo
- `discussion-notes-structure-and-magnitudes.md` — earlier draft essay (superseded by the memo)
- `discussion-notes-logic-of-two-bits.md` — notes from Session 3 exploring the economic logic of the two-bit result

## Status

- Revised memo sent to coauthors (Fellingham, Lin, Schroeder) — awaiting responses
- Session 3 produced a potentially important economic interpretation of the two-bit result: two independent dimensions (cash effect and equity effect)
- This interpretation needs to be checked against the paper's formal structure
- The proofs have not yet been examined in detail — still a priority for future sessions

## How to resume

1. Read this file first.
2. Read `discussion-notes-logic-of-two-bits.md` for the economic interpretation of the two-bit result developed in Session 3.
3. Read `memo-structure-and-magnitudes.md` for the proposed new introduction and supporting reasoning from Session 2.
4. Read the proofs in `Info-Property-Double-Entry.md` — Appendix A starts around line 835. Key proofs: Proposition 2 (~line 835), Theorem (~line 1039).
5. Rick's thoughts are also in his Open Brain — search for "double entry" or "equity boundary" or "structural capacity" or "Z operator" or "revaluation" or "two independent dimensions" or "cash effect equity effect."
