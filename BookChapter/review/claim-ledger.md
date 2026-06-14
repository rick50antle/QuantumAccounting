# Claim Ledger for Chapter.docx

Working file: /Users/ra1/QuantumAccounting/BookChapter/sources/Chapter.original.docx

Extracted chapter text: /Users/ra1/QuantumAccounting/BookChapter/extracted/Chapter.original.extracted.md

## Sources Reviewed

- Quantum programming source: /Users/ra1/QuantumAccounting/BookChapter/sources/Quantum Programming January 19 2026.docx
- Odd-cycle source: /Users/ra1/QuantumAccounting/BookChapter/sources/Entanglement and Odd Cycle Game draft 02-12-2026.docx
- Information property source: /Users/ra1/QuantumAccounting/BookChapter/sources/Info-Property-Double-Entry-202503.docx
- Existing quantum-programming technical review: /Users/ra1/QuantumAccounting/QuantumProgramming/quantum_programming_review.txt
- Existing odd-cycle review notes: /Users/ra1/Library/CloudStorage/OneDrive-YaleUniversity/AFLS_Paper/LinFellingham/Review_Suggestions.md
- Information-property discussion notes in /Users/ra1/QuantumAccounting/InfoPropDoubleEntry
- External primary checks: Aharonov arXiv:quant-ph/0301040 and Shi arXiv:quant-ph/0205115
- External odd-cycle check: Drmota et al. arXiv:2406.08412

## Status Key

- Supported: source result appears to justify the claim as written or with only ordinary citation support.
- Revise: underlying idea is usable, but current wording is too broad, imprecise, or underexplained.
- Verify: cited source was not in the working packet or the extracted files omit needed formal details.
- Remove or Recast: current claim is likely misleading unless substantially reframed.

## Ledger

| ID | Chapter Location | Claim | Support Check | Status | Revision Action |
| --- | --- | --- | --- | --- | --- |
| C01 | Ch. lines 19-23 | The double-entry system remains relevant in the quantum era because its structure can represent fundamental quantum operations. | Supported by the quantum-programming source, but only as a representation or notation, not as physical quantum computation. | Revise | Keep the thesis, but state that double-entry provides a classical representational language for quantum information structures. |
| C02 | Ch. lines 23, 235 | The advantage of quantum computing highlights advantages of double-entry over single-entry. | The analogy is promising but not automatically entailed by the gate representation. It is supported mainly by the channel-capacity and odd-cycle models. | Revise | Make the bridge explicit: "in stylized information-processing models, the relational structure of double entry can outperform scalar/single-entry representations." |
| C03 | Ch. lines 25, 37-65 | Decision-making, accounting numbers, and entropy are alternative representations of the same activities. | This cites Fellingham et al. 2022, which is not in the source packet. The chapter's equations were not extracted clearly enough to verify. | Verify | Treat this as prior literature, not as something the chapter proves. Add a plain-English bridge before the equations. |
| C04 | Ch. lines 43-55 | Kelly/log-growth/accounting equivalence supports the information-science framing. | Plausible, but the formal equations are missing from extraction and the underlying 2022 source is not included. | Verify | Either provide a short derivation from the cited source or move detail to a footnote and keep the main text intuitive. |
| C05 | Ch. line 65 | The equivalence extends to quantum probabilities. | Not verified from the packet. This is a high-risk bridge because quantum measurement is not just Bayesian updating. | Verify | Use cautious wording: "the cited work argues..." and distinguish Bayesian conditionalization from quantum state update. |
| C06 | Ch. lines 67-69 | Double-entry can process classical probability rules and may process quantum probability rules. | "May process" is safer than "can process." The quantum-programming source uses accounting notation plus external amplitude bookkeeping. | Revise | Say the framework can encode selected quantum-information structures, with probabilities carried by separately tracked amplitudes. |
| C07 | Ch. lines 73-93 | T-accounts encode qubit basis states and journal entries encode X, Z, S, and T-style operations. | Supported by quantum-programming source lines 63-105. | Supported | Retain, but add a roadmap table so nonexperts can track the mapping. |
| C08 | Ch. lines 81-93 | Quantum gates are reversible unitary operations; journal entries preserve information analogously. | Reversibility claim is broadly correct for closed quantum systems, but reversibility is not unique to quantum computation. | Revise | Avoid saying reversibility explains quantum superiority. Say it is one shared structural feature of unitary circuits and reversible accounting transformations. |
| C09 | Ch. lines 97-105 | The Hadamard gate creates superposition; accounting notation stacks E and A rows. | Supported, but the accounting notation is incomplete unless amplitudes and normalization are specified. | Revise | Add "the account notation records basis-state structure while amplitudes are recorded separately." |
| C10 | Ch. line 105 | Superposition allows information to be carried by two financial statements simultaneously. | This is an interpretive analogy, not a literal quantum statement about financial statements. | Revise | Recast as: "the notation represents information across multiple linked statement rows, analogous to a superposition over basis states." |
| C11 | Ch. lines 109-111 | Composite systems are represented by concatenated accounts or tensor products. | Must be stated carefully. In quantum mechanics, the state space of a composite system is the tensor product of state spaces; not every state factors as a tensor product. | Revise | Correct the postulate language. Product basis states can be concatenated, but entangled states are superpositions of product states. |
| C12 | Ch. line 111 | CNOT transforms AEA into AAA when the first account controls the second. | This particular example is consistent with E = 0, A = 1, control = first, target = second. | Supported | Retain. Avoid inheriting the reversed CNOT example flagged in the quantum-programming source review. |
| C13 | Ch. lines 117-119 | Toffoli is universal for classical reversible computation and Toffoli plus Hadamard is universal for quantum computation. | Supported by Aharonov arXiv:quant-ph/0301040 and Shi arXiv:quant-ph/0205115. | Supported | Retain exact claim, but add "approximate arbitrary unitaries/circuits to arbitrary accuracy" if using the quantum universality claim. |
| C14 | Ch. line 119 | Since double-entry encodes H and Toffoli, it is universal for classical and quantum computation. | This is too strong as written. The source supports representational encoding of a universal gate set, not that the double-entry system itself is a computational device. | Revise | Say "the framework can represent a universal gate set" and "therefore has the representational vocabulary needed to describe universal quantum computation." |
| C15 | Ch. line 121 | Symmetry, balance, and reversibility explain the capacity. | Plausible conjecture, not a theorem in the sources. | Revise | Label as conjecture or interpretive explanation. Tie channel-capacity advantage more directly to articulation and relational structure. |
| C16 | Ch. line 123 | The superiority of quantum computers over classical computers arises largely from entanglement. | Overbroad. Entanglement is a key resource in many quantum advantages, but not the sole or universal explanation. | Remove or Recast | Use "Entanglement is one defining resource in many quantum information tasks." |
| C17 | Ch. lines 129-139 | Bell states can be generated by H followed by CNOT and represent nonseparable account relationships. | Supported by the odd-cycle source and standard quantum theory. | Supported | Retain, but explain "nonseparable" before "nonlocal" for nonexpert readers. |
| C18 | Ch. lines 145-185 | Entanglement gives two-bit channel capacity by allowing four journal-entry messages to be distinguished through operations on one account. | Supported by the information-property source, with a qualification: the original paper frames the mechanism as superposition plus articulation; "Bell state" language is analogical and appears in Appendix B. | Revise | State the accounting conditions precisely: two articulating statement rows and at least two accounts satisfying the articulation identities. |
| C19 | Ch. line 185 | n-bit channel capacity is achieved with n entangled accounts. | The information-property source supports n-bit capacity under specific n-account/two-statement articulation conditions. | Revise | Replace with: "in the n-account extension, the model produces n bits when all n accounts satisfy the articulation conditions." |
| C20 | Ch. lines 189-203 | Classical 3-seat odd-cycle maximum is 5/6; entangled case reaches 1/2 + sqrt(3)/4; superposition without entanglement reaches 1/2. | Supported by the odd-cycle source. The exact quantum value equals cos^2(pi/12). Drmota et al. gives the general odd-cycle quantum limit cos^2[pi/(4n)]. | Supported | Use exact value first, approximation second. Add a simple nontechnical explanation of why 5/6 is the classical ceiling. |
| C21 | Ch. lines 205-207 | Entanglement is the source of coordination advantage; superposition without entanglement can be detrimental. | Supported within the specific three-case odd-cycle model. | Revise | Add "in this model" and avoid generalizing to all quantum strategies or all organizational settings. |
| C22 | Ch. line 209 | The classical odd-cycle game is analogous to single-entry, while the quantum version is analogous to double-entry. | This is interpretive, not a theorem. It can be valuable if framed as an analogy. | Revise | Say "suggests an analogy" and clarify that double-entry remains a classical accounting architecture. |
| C23 | Ch. lines 213-227 | In agency settings, entanglement is a productive resource and group measurement can dominate individual measurement under synergy. | The Demski et al. 2008 source is cited but not included in the working packet. The chapter maps synergy to entanglement, which is interpretive. | Verify | Keep the Demski result only if the original paper is checked. Soften "entanglement contributes directly to production" to "relational measurement preserves information about joint production." |
| C24 | Ch. lines 225-227 | More severe agency problems expand the range over which group measurement dominates. | Not verified from the packet. | Verify | Check Demski et al. 2008 before making this a major conclusion. |
| C25 | Ch. lines 231-237 | The chapter shows double-entry supports vector processing, superposition, and entanglement. | The chapter can show formal analogues, not literal physical quantum properties. | Revise | Use "admits a vector representation," "has a structural analogue of superposition," and "can model nonseparable relational structures." |
| C26 | Ch. lines 233-235 | Double-entry processes information in a way that cannot be achieved classically. | Misleading because double-entry is classical. The intended comparison is against scalar/single-entry representations under specific models. | Remove or Recast | Say "cannot be achieved by the corresponding scalar/single-entry representation in these models." |
| C27 | Ch. line 235 | The analysis explains the durability of double-entry over five centuries. | Too strong as a historical causal claim. The result offers one information-theoretic explanation, not a complete historical explanation. | Revise | Use "offers one reason" or "helps explain." |
| C28 | Ch. line 237 | The framework has pedagogical value for researchers, educators, and practitioners. | Supported as a reasonable conclusion if overstatements are controlled. | Supported | Retain. It may become a stronger closing than the broad "quantum era" claim. |

## Highest-Priority Corrections

1. Change the main claim from "double-entry is universal for quantum computation" to "double-entry can represent a universal quantum gate set when paired with explicit amplitude bookkeeping."
2. Replace literal-sounding claims of accounting entanglement/superposition with "structural analogues" unless a formal Bell-state model is actually being used.
3. Add exact conditions to the channel-capacity result: two statement rows, at least two accounts, and articulation identities.
4. Treat Section 1 and Section 3.4 as citation-dependent until Fellingham et al. 2022 and Demski et al. 2008 are checked.
5. Reframe the conclusion around "articulation as code": information lives in relationships among accounts/statements, not merely in individual balances.
