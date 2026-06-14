# Pre-Submission Review: "Double-entry Accounting, Entanglement, and Odd-cycle Game"

**Reviewer notes for: Antle, Fellingham, Lin, and Schroeder**
**Date: February 20, 2026**

---

## Overall Assessment

This paper presents a genuinely original contribution: it uses the odd-cycle game to demonstrate that double-entry accounting, interpreted as a vector-processing system, can outperform single-entry (scalar) processing when divisions are connected through articulation constraints. The analogy between quantum entanglement and cross-divisional articulation is both surprising and illuminating. The mathematical analysis is largely correct (verified computationally), and the three-case comparison---classical baseline, entangled, and superposition without entanglement---tells a compelling story.

That said, the manuscript in its current form reads more like a working draft than a journal submission. The issues below range from structural omissions (no abstract, no conclusion, a one-sentence introduction) to presentation choices that may alienate the accounting audience the paper most needs to reach.

---

## 1. Major Structural Issues

### 1.1 Missing Abstract

The paper has no abstract. Every accounting journal requires one. A well-crafted abstract (150--200 words) should state the research question, the method (odd-cycle game with quantum strategies), the key finding (entangled double-entry achieves ~93.3% versus the classical 83.3% ceiling), and the implication for accounting system design.

### 1.2 The Introduction Is a Single Sentence

The introduction currently reads: *"The purpose of this paper is to offer one explanation why double-entry system is superior to single-entry system in a simple odd-cycle game with restricted information channel."*

This needs to become a full section (roughly 2--4 pages) that accomplishes several things: motivates the question of *why* double-entry has persisted for centuries, situates the paper relative to the existing accounting information systems literature, explains what the odd-cycle game is and why it provides a useful test, previews the three main results and their accounting interpretation, and signals the paper's contribution clearly. The reader should understand, before encountering any formalism, why this paper matters.

### 1.3 The Conclusion Says "To Be Added Later"

Section IV is a placeholder. The concluding section should summarize the main findings, discuss limitations (the game is stylized; the analogy is structural rather than literal), suggest directions for future research (e.g., games with more seats, connections to consolidation practices, empirical predictions), and reiterate the paper's contribution to accounting theory.

### 1.4 The Reference List Has Only Three Entries

Three references will not survive peer review. The paper should engage with the literature on accounting information systems (e.g., Ijiri's foundational work on double-entry structure; Fellingham and Schroeder's prior work on quantum accounting), the odd-cycle game in the quantum information literature (the paper cites Drmota et al. 2025 but not the original theoretical work by, e.g., Galliard, Tapp, and Wolf 2003 or Brassard, Broadbent, and Tapp 2005), and the broader question of why double-entry persists (e.g., Ijiri 1967, Mattessich 1964, Demski 2004). A related-literature section or an expanded introduction that weaves in this context would strengthen the paper substantially.

### 1.5 Section Numbering Is Inconsistent

The paper uses Roman numerals for top-level sections (I, II, III, IV) but then switches to decimal numbering (3.1, 3.2, 3.3) within Section III. Pick one convention and apply it uniformly.

---

## 2. Presentation for an Accounting Audience

### 2.1 The Paper Needs More Scaffolding Before the Formalism

The paper's target readers are accounting researchers, most of whom will not have background in quantum information theory. Currently, the paper jumps from the classical game setup (Section II) directly into "Definition 1 (Accounting representation of qubit states)" with kets, tensor products, and Hadamard gates. There should be an intuitive bridge between Section II and Section 3.1---perhaps a paragraph that says something like: "We now introduce a formal framework, developed in Fellingham et al. (2026), that represents quantum operations using accounting constructs. The key insight is that double-entry bookkeeping has structural features---superposition across multiple statements, coordinated entries---that parallel the structure of quantum computation."

### 2.2 Appendix B Is More Accessible Than the Main Paper

Appendix B does an excellent job of explaining what scalar versus vector processing means, why articulation creates a structural constraint analogous to normalization in quantum mechanics, and what the three cases imply for accounting system design. Much of this material---particularly Sections B.1, B.5, and B.7---should be *in the main paper*, not buried in an appendix. Consider moving the core accounting interpretation from the appendix into Section 3.3, and reserving the appendix for the more technical elaboration.

### 2.3 The Accounting Interpretation Section (3.3) Needs Expansion

Section 3.3 is the payoff for an accounting reader, and it currently feels compressed. Definition 7 (articulation), Definition 8 (superposition property), and Definition 9 (entanglement property) are introduced in rapid succession with relatively little discussion. Each of these definitions deserves a paragraph of interpretation. The connection between articulation identities and superposition constraints is the conceptual heart of the paper---give it room to breathe.

### 2.4 Relate the Three Cases Explicitly to Accounting Scenarios

The paper would benefit enormously from a summary table (like the one in Appendix B, Section B.5) placed in the main text. The table mapping Case 1 to independent single-entry ledgers, Case 2 to integrated double-entry with cross-divisional articulation, and Case 3 to disconnected double-entry would give accounting readers an immediate anchor for the mathematical results.

---

## 3. Technical and Mathematical Issues

### 3.1 Precision in Proposition 2

Proposition 2 states the maximum winning probability as "0.933." For a formal result, use the exact expression: cos^2(pi/12) = (2 + sqrt(3))/4. The approximation can follow in parentheses. The proof correctly derives 1/2 + sqrt(3)/4, which equals cos^2(pi/12)---state this equivalence explicitly, as it connects your result to the standard quantum information literature.

### 3.2 The Proof of Lemma 1 Could Be Tighter

The mixed-strategy argument in the proof of Lemma 1 considers mixing between strategies RRB and RBB specifically. The final paragraph generalizes correctly (since any mixed strategy is a convex combination of pure strategies, and all pure strategies achieve at most 5/6, the mixed strategy cannot exceed 5/6). However, the specific two-strategy calculation contains a claim that Prob(winning|RBB,RRB) = 3/6. This is correct but should be verified explicitly in the text (showing which seat assignments are won and lost under this strategy pair), since the paper only shows the calculation for Prob(winning|RRB,RBB) = 5/6 in detail.

Also, the final inequality states p + (1-p)q < 1 when q < 1, yielding Prob(winning) < 5/6 strictly. But the paper earlier claims the bound is *attainable* at 5/6. The mixed-strategy analysis shows strict inequality only for interior mixing probabilities. A cleaner statement: "No mixed strategy achieves a winning probability strictly greater than 5/6, and the bound 5/6 is attained by the pure strategies identified above."

### 3.3 Symmetry Assumption in Proposition 2 Proof

In the proof of Proposition 2, the paper assumes x_0 = x_1 "due to the symmetry of f(.)." This needs a sentence of justification. The function f(x_0, x_1) = |sin(x_0)| + |sin(x_1)| + |sin(x_0 + x_1)| subject to x_2 = -(x_0 + x_1) is symmetric in x_0 and x_1, so the maximum can indeed be sought along x_0 = x_1 without loss of generality. But the reader should be told why.

### 3.4 Notation for Phase Angles

The paper defines phase-shift angles as theta in [0, 2pi], but the proof of Proposition 2 produces optimal angles that include negative values (theta_22 = -2pi/3). Either expand the domain to include negative angles, or note that angles are defined modulo 2pi and -2pi/3 is equivalent to 4pi/3.

### 3.5 Minor Probability Computation in Case 3

In the proof of Proposition 3, the probability computation for Prob(EE) contains a small notational issue. The expression 2(1 - e^{i*theta_2*pi}) * 2(1 + e^{-i*theta_2*pi}) uses a bullet (.) for multiplication between the amplitude and its conjugate. The amplitude for EE should be 2(1 - theta_2) from the evolution, and its conjugate 2(1 - theta_2*), giving 4|1 - e^{i*theta_2*pi}|^2 = 4[2 - 2cos(theta_2*pi)]. The computation arrives at the correct answer, but the intermediate step mixes the amplitude and conjugate terms in a way that could confuse a careful reader---specifically, (1 - e^{i*theta}) * (1 + e^{-i*theta}) != |1 - e^{i*theta}|^2. Check whether this is a typo or an intentional algebraic shortcut. **[Update: looking more carefully, the amplitude for EE appears to be 2(1 - theta_2), whose complex conjugate is 2(1 - e^{-i*theta_2*pi}). The paper writes (1 + e^{-i*theta_2*pi}) which would be the conjugate of (1 - e^{i*theta_2*pi}) only if there were no sign error. This deserves a careful re-check.]**

---

## 4. Writing and Style

### 4.1 Grammatical Issues

Several places have missing articles or minor grammatical issues. For example:

- "why double-entry system is superior to single-entry system" should read "why **the** double-entry system is superior to **the** single-entry system" (or "**a** double-entry system")
- "Similar, applying the two operators..." (line near Definition 6) should be "**Similarly**, applying..."
- "There are four Ball states" should be "There are four **Bell** states" (typo in Definition 6)
- "the number of reports equals the number of seats)" has an unmatched closing parenthesis in Section II
- "A subsequent reclassification entry such as depreciation reduces..." --- depreciation is typically a *revaluation* entry in the paper's own terminology (Definition 2), not a reclassification
- "financial statement:" at the end of Section 3.3 should be "financial statement**s**:"

### 4.2 Notation Consistency

The paper uses both "cos theta_1 pi cos theta_2 pi" (product of cosines) and "cos(theta_1 + theta_2)pi" (cosine of sum) without always being careful about parentheses. Consider using cos(theta_1 * pi) * cos(theta_2 * pi) and cos((theta_1 + theta_2) * pi) consistently to avoid ambiguity about what is inside the cosine.

### 4.3 Equation Numbering

The paper numbers very few equations (only (1), (2), (3) in Section 3.3, and (A1)--(A3) in the proof of Proposition 2). For a paper this equation-heavy, number all displayed equations. This makes cross-referencing far easier during peer review.

---

## 5. Suggestions for Strengthening the Contribution

### 5.1 Discuss the Drmota et al. (2025) Experimental Result

The paper cites Drmota et al. (2025), which reports experimental confirmation of quantum advantage in the odd-cycle game using trapped-ion qubits. This is a powerful validation---the advantage your paper attributes to double-entry structure has been physically realized in a laboratory. Mention this explicitly, as it strengthens the claim that the advantage is not merely mathematical curiosity.

### 5.2 Connect to the Broader "Why Double-Entry?" Question

Accounting historians have long puzzled over why double-entry bookkeeping became universal. Existing explanations emphasize error detection, stewardship, and legal compliance. Your paper offers a fundamentally different explanation: double-entry provides a structural information-processing advantage that single-entry cannot replicate. This is a strong claim and should be positioned as such in the introduction and conclusion.

### 5.3 Discuss Limitations Explicitly

The odd-cycle game is a specific coordination game with a specific structure. Readers will want to know: Does the advantage generalize to games with more than 3 seats? To other types of coordination problems? Is the analogy between quantum entanglement and accounting articulation formal or metaphorical? Being upfront about these limitations will strengthen rather than weaken the paper.

### 5.4 Consider Adding a Simple Numerical Example

Before or alongside the formal analysis, a worked numerical example showing how the quantum strategy achieves 93.3% in a specific instance (using the optimal angles from Proposition 2) would make the result tangible for accounting readers. Walk through one seat assignment, show the journal entries, show the measurement probabilities, and show how they differ from the classical case.

---

## 6. Summary of Priority Actions

**Must-fix before submission:**

1. Add an abstract
2. Expand the introduction (motivation, literature, contribution statement, paper outline)
3. Write the conclusion (Section IV)
4. Fix the "Bell/Ball" typo in Definition 6
5. Fix the unmatched parenthesis in Section II
6. Expand the reference list substantially
7. Make section numbering consistent

**Strongly recommended:**

8. Move key accounting interpretation material from Appendix B into the main text
9. Add the summary table from Appendix B (Section B.5) to the main paper
10. Add more intuitive explanation before and after the formal definitions
11. Express Proposition 2's result in exact form: cos^2(pi/12)
12. Number all displayed equations
13. Add a worked numerical example
14. Tighten the proof of Lemma 1 regarding mixed strategies
15. Verify the sign in the Prob(EE) computation in Proposition 3's proof

**Nice to have:**

16. Discuss Drmota et al. (2025) experimental results more prominently
17. Add a section on limitations and future directions
18. Clean up notation for trigonometric expressions (consistent parenthesization)
19. Discuss how the result connects to classical accounting theory (Ijiri, Mattessich)
