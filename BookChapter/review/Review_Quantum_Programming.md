# Pre-Submission Review: "Using Double-Entry Accounting to Program Quantum Computers"

**Reviewer notes for: Fellingham, Lin, and Schroeder**
**Date: February 20, 2026**

---

## Overall Assessment

This paper is substantially more polished than the companion odd-cycle game paper and makes a genuinely compelling argument: the double-entry system, with its T-accounts and journal entries, provides a natural and complete representation of quantum computing primitives. The construction of the Toffoli gate using accounting notation is the paper's centerpiece, and it works. The A circle / E circle framework is elegant, and the step-by-step Toffoli demonstrations are pedagogically effective.

That said, the paper contains one clear technical error in the CNOT example, several typos, and some structural choices (particularly the heavy reliance on footnotes) that could be improved before journal submission. The issues below are organized by severity.

---

## 1. Technical Error: CNOT Example Is Reversed

In the paragraph following Definition 7, the paper states:

> "the CNOT gate changing |10⟩ into |11⟩ is written as AA → AE"

This is incorrect. By the paper's own definitions (E = |0⟩, A = |1⟩, and |01⟩ = EA), we have |10⟩ = AE and |11⟩ = AA. The CNOT gate with control qubit 1 (which is A, on the A circle) should flip qubit 2 from E to A, giving AE → AA. The paper has the accounting notation backwards: AA → AE actually represents |11⟩ → |10⟩, which is the reverse operation.

I verified this computationally against the standard CNOT truth table. The corrected text should read: "the CNOT gate changing |10⟩ into |11⟩ is written as AE → AA, meaning that given the first account is A, perform the X-gate on the second account and change it from E to A."

This error does not propagate into the Toffoli gate analysis (which was verified separately), but it should be fixed as it appears in a definitional example.

---

## 2. Typos and Grammatical Errors

The following errors should be corrected:

- **"first wo qubits"** (Section IV, Toffoli gate truth table discussion): should be "first **two** qubits"
- **"interpretating"** (Introduction, para 4): should be "**interpreting**"
- **"interpretated"** (Section 2.3, Accounting Interpretation): should be "**interpreted**"
- **"Noted that"** (footnotes 12 and 15): should be "**Note** that"
- **"single-entry system"** (final sentence of Concluding Remarks): should be "single-entry **systems**" (plural, to match "double-entry systems" earlier in the sentence)
- **"Anil, A."** (References, first entry): should likely be "**Arya**, A." — the text cites "Arya et al 2000" but the reference lists "Anil, A." The author's name is Anil Arya, so the reference should be formatted as "Arya, A." with "Anil" as the given name

---

## 3. Structural Issues

### 3.1 Excessive Footnotes

The paper has 26 footnotes. Many are substantive — footnote 17 alone contains a full-page matrix computation. For an accounting journal, this volume of footnotes is distracting and signals material that either belongs in the main text or in an appendix. Recommendations:

- Footnotes 1, 3, 4, 7, and 24 contain important conceptual points. Incorporate their substance into the main text (at least partially).
- Footnote 17 (the long matrix verification) should become an appendix. It's valuable for verification but interrupts the reading flow.
- Footnotes that are purely parenthetical (e.g., footnotes 5, 13, 22, 23) can remain as footnotes or be converted to brief in-text parenthetical remarks.

### 3.2 Section Numbering Inconsistency

The top-level sections use Roman numerals (I, II, III, IV, V), but subsections use a mix of formats: "2.1" and "2.2" appear with inconsistent formatting (some italic, some not; "2." vs "2.2"), while Section III uses "3.1", "3.2", "3.3", "3.4". Standardize the numbering throughout.

### 3.3 Section 3.4 (Measurement) Is Underdeveloped

This section introduces Postulate 4 and Definition 11 but then says "Measurement is not the focus of this paper." This is fine as a scope decision, but the section feels perfunctory. Either expand it slightly (e.g., a brief worked example of measurement on a single superposition state using the accounting notation) or signal earlier in the paper that measurement will be treated in a companion paper. The current treatment may leave reviewers feeling the coverage of the four postulates is incomplete.

### 3.4 Reference Formatting Is Inconsistent

Some references use "Vol." and explicit page ranges, others don't. Some have parenthetical volume numbers, others use colons. Standardize to the target journal's citation format. Specific issues:

- "Anil, A." → "Arya, A." as noted above
- "Antle, R., Fellingham, J., H. Lin..." — inconsistent use of initials (some authors get first initial only, others get full names)
- Pelaez (2021) is a Medium blog post. Consider whether this is appropriate for the target journal; the phase kickback concept can also be cited from a textbook source.
- "Fellingham et al. (2025)" is cited in footnote 16 but the reference lists "Antle, R., Fellingham, J., H. Lin, and D. Schroeder. 2025." — the in-text citation should be "Antle et al. (2025)" to match the reference's first author.

---

## 4. Presentation Suggestions

### 4.1 The Introduction's Final Paragraph

The claim that "the double-entry system can be viewed, not only as the language of quantum computers, but also as the language of the universe itself" via Lloyd (2006) is memorable but may strike some reviewers as over-reaching. Consider softening it slightly — perhaps framing it more explicitly as speculative ("One might speculate that...") or placing it in the conclusion rather than the introduction, where it may color reviewers' initial impression of the paper's rigor.

### 4.2 The Toffoli Gate Section Could Use a Summary

After the two step-by-step examples, a brief paragraph summarizing the pattern would help readers extract the key insight without re-reading the long chains of operations. The existing summary at the end (the six-point "(i)...(vi)" list) does this partially but could be more explicitly positioned as a high-level description before the detailed examples.

### 4.3 The Recomposition Operation Deserves More Motivation

Definition 10 introduces recomposition entries, which are important for the Toffoli gate construction. However, the motivation ("fractional revaluations can be loaded entirely on the last qubit") could benefit from an additional sentence explaining *why* this simplification matters — namely, that it reduces the bookkeeping complexity of multi-qubit programs and mirrors the phase kickback technique in quantum computing (currently relegated to footnote 20).

### 4.4 Consider Adding a "Roadmap" Table

A table mapping quantum constructs to their double-entry counterparts (qubit → T-account, gate → journal entry, measurement → closing entry, etc.) placed at the end of the introduction would give readers a one-page reference card for the rest of the paper. This would be especially valuable for accounting readers who will repeatedly need to recall which quantum concept maps to which accounting construct.

---

## 5. Minor Mathematical/Notational Issues

### 5.1 Amplitude Recording Convention

The paper states that amplitudes are "recorded separately" (Definitions 8 and 11) but never specifies a systematic convention for how this recording works in a multi-qubit, multi-operation program. Reviewers may ask: how does one track the 1/√2 normalization through a sequence of Hadamard gates and conditional operations? A brief remark (even a single sentence) explaining that the accounting notation tracks the state structure while amplitudes are maintained as a separate normalization constant would preempt this question.

### 5.2 The Notation A^(k/4) and Â^(k/4)

The fractional superscript notation is well-defined in the text but can be visually confusing in the step-by-step Toffoli calculations, especially when combined with hats. Consider whether a table listing all accounts on the A circle with their corresponding quantum states (e.g., A^(1/4) = e^{iπ/4}|1⟩) would help readers follow the long computation chains.

---

## 6. Summary of Priority Actions

**Must-fix before submission:**

1. Correct the CNOT example (AA → AE should be AE → AA)
2. Fix "first wo qubits" → "first two qubits"
3. Fix "interpretating" → "interpreting"
4. Fix "interpretated" → "interpreted"
5. Fix "Anil, A." → "Arya, A." in references
6. Fix "Noted that" → "Note that" (footnotes 12 and 15)
7. Fix "single-entry system" → "single-entry systems" (conclusion)
8. Fix "Fellingham et al. (2025)" → "Antle et al. (2025)" in footnote 16

**Strongly recommended:**

9. Reduce footnote count — move substantive footnotes into text, move footnote 17 to appendix
10. Standardize section numbering
11. Standardize reference formatting
12. Expand Section 3.4 (Measurement) or signal its limitations earlier
13. Add a roadmap table mapping quantum ↔ accounting constructs

**Nice to have:**

14. Soften the Lloyd "language of the universe" claim
15. Add a summary paragraph before the Toffoli step-by-step examples
16. Motivate the recomposition operation more fully
17. Add a table of all A-circle accounts with their quantum states
18. Replace the Pelaez (2021) Medium citation with a textbook reference
