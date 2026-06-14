# Red-Team Proof Audit Memo

Working document: Chapter.rewritten.hardened.docx

Purpose: classify the chapter's important claims by proof status, identify what supports each claim, and state wording guardrails that keep the chapter accurate.

## Executive Verdict

The hardened chapter is defensible if it maintains one central distinction: double entry is not claimed to be quantum machinery. It is claimed to be a classical relational information architecture that can represent selected quantum-information structures and that, in the reviewed models, can preserve information unavailable to isolated scalar records.

The strongest supported claims are the representational gate-set claim, the two-bit channel-capacity result under articulation conditions, and the three-seat odd-cycle comparison. The highest-risk claims are the decision/accounting/information equivalence and the agency-performance section because those depend on sources not included in the working packet. They should remain in the chapter as cited prior literature or organizational analogy, not as newly proved results.

## Claim-Type Key

- Established result: a theorem, proposition, or calculation in the reviewed source papers or standard quantum-information literature.
- Representation claim: a claim that double-entry notation can encode, model, or display a formal structure.
- Interpretive analogy: a useful accounting or organizational interpretation of a formal model, but not an identity.
- Speculative implication: a forward-looking or explanatory inference that should be stated cautiously.

## Audit Register

### A01. Core Thesis: Double Entry As Relational Information Architecture

Type: Interpretive synthesis.

Support: The information-property paper models accounting as a communication channel; the quantum-programming paper represents gates with accounting objects; the odd-cycle paper uses relational/Bell-state structure to model coordination.

Risk: Could sound like a historical proof that double entry survived because of quantum-like properties.

Guardrail: Say the chapter offers one information-theoretic explanation for double entry's durability, not a complete historical cause.

Chapter treatment: Keep. The hardened thesis is appropriately cautious.

### A02. Decision, Accounting, And Information Equivalence

Type: Established result by citation, but not independently rechecked in this working packet.

Support: Fellingham, Lin, and Schroeder (2022) as cited in the chapter.

Risk: The chapter could appear to reprove or extend the 2022 result, especially if it connects classical information measures too quickly to quantum probabilities.

Guardrail: Treat the result as prior literature. Do not use it to claim that quantum measurement is merely Bayesian updating.

Chapter treatment: Keep as framing only. The formal note correctly says the chapter uses this result rather than reproving it.

### A03. Qubit Basis States And Account Labels

Type: Representation claim.

Support: Quantum-programming source defines E and A as basis-state/account labels and uses journal entries as operators.

Risk: Readers may infer that real accounts are physical qubits.

Guardrail: Always say "basis labels," "representation," or "notation." Avoid "accounts are qubits."

Chapter treatment: Keep. The amplitude-bookkeeping caveat is essential.

### A04. X, Z, S, T, And Hadamard Gate Representations

Type: Representation claim supported by source constructions.

Support: Quantum-programming source and information-property source both use X and Z; quantum-programming source uses phase and Hadamard constructions.

Risk: Hadamard and phase claims become misleading if amplitudes, normalization, and relative phase are omitted.

Guardrail: State that account labels carry basis structure while amplitudes and probabilities are tracked separately.

Chapter treatment: Keep. The hardened draft states this caveat repeatedly.

### A05. Composite Systems, Tensor Products, And Entanglement

Type: Established quantum-information result plus representation claim.

Support: Standard quantum theory; odd-cycle source's Bell-state construction.

Risk: Saying "the state of the whole is the tensor product of the states of the parts" would exclude entanglement.

Guardrail: Say the state space is the tensor product of component spaces; product basis states concatenate; general states may be entangled superpositions.

Chapter treatment: Keep. The correction is already in the layered and hardened drafts.

### A06. Representational Universality

Type: Established theorem plus representation claim.

Support: Aharonov (2003) and Shi (2003) for Toffoli plus Hadamard universality; quantum-programming source for accounting representations of the relevant gates.

Risk: "Double entry is universal for quantum computation" overstates the result.

Guardrail: Say the framework can represent a universal gate set when paired with explicit amplitude bookkeeping. Do not say it physically implements quantum computation.

Chapter treatment: Keep. Proposition 1 is correctly framed as representational.

### A07. Bell States As Nonseparable Relationships

Type: Established quantum-information result plus interpretive accounting analogy.

Support: Odd-cycle source constructs Bell states from Hadamard plus CNOT; standard rank/separability logic.

Risk: "Accounts are entangled" sounds literal.

Guardrail: Say Bell states model nonseparable relationships; articulation is the accounting analogue.

Chapter treatment: Keep. The appendix proof sketch is appropriate.

### A08. Two-Bit Channel Capacity

Type: Established source result.

Support: Information-property paper, especially Proposition 2, Proposition 3, and the theorem: two-bit capacity requires two statement rows, at least two accounts, and articulation identities.

Risk: The result may be overstated if magnitudes are not mentioned, if one ignores the signal-equivalence rule, or if "more accounts" is treated as sufficient.

Guardrail: State the model assumptions: scale is abstracted away; messages are I, X, Z, and XZ; scalar multiples are not distinct signals; two-bit capacity requires linked rows and qualifying account columns.

Chapter treatment: Keep. The new worked example makes the collapse mechanism visible.

### A09. N-Account Scaling

Type: Established source result, but easy to blur with the one-account/two-bit theorem.

Support: Information-property paper's n-account extension.

Risk: "An n-account structure gives n bits" is too broad unless the expanded message space and articulation conditions are specified.

Guardrail: Distinguish the claims: one account can transmit two bits when embedded in an articulated structure with at least two qualifying accounts; the n-bit extension applies when the n-account message structure is used and all relevant columns satisfy the articulation identities.

Chapter treatment: Keep after the hardened wording change.

### A10. Classical Odd-Cycle Ceiling

Type: Established source result.

Support: Odd-cycle source Lemma 1 and appendix proof.

Risk: The result may look like a hand-wavy coloring story unless the six assignments are stated.

Guardrail: Say there are three same-seat and three adjacent-seat assignments; any two-coloring of a three-cycle fails at least one adjacent edge; therefore at most five of six can be won.

Chapter treatment: Keep. The chapter gives the intuitive proof and the appendix states the calculation.

### A11. Entangled Odd-Cycle Advantage

Type: Established source result.

Support: Odd-cycle source Proposition 2; external odd-cycle literature supports the general form.

Risk: Generalizing from this game to all coordination problems or all uses of superposition.

Guardrail: Use "in this model" and "with the specified Bell-state strategy." Preserve the exact value 1/2 + sqrt(3)/4 = cos^2(pi/12), approximately 0.933.

Chapter treatment: Keep. Proposition 4 is properly narrow.

### A12. Superposition Without Entanglement Performs Worse

Type: Established source result within the specified model.

Support: Odd-cycle source Proposition 3.

Risk: Could be misread as "superposition is bad" generally.

Guardrail: Say superposition without the relevant relational link performs worse in this model.

Chapter treatment: Keep. The comparison table is useful.

### A13. Single-Entry Versus Double-Entry Analogy

Type: Interpretive analogy.

Support: Odd-cycle paper's accounting interpretation, but the mapping from classical/quantum strategies to single-entry/double-entry is analogical.

Risk: Saying the quantum game "is" double entry or the classical game "is" single entry.

Guardrail: Use "resembles," "suggests an analogy," and "in the model."

Chapter treatment: Keep with caution. The hardened chapter already says the analogy is useful but limited.

### A14. Agency And Performance Measurement

Type: Cited prior result plus interpretive analogy.

Support: Demski, Fellingham, Lin, and Schroeder (2008), not included in the working packet.

Risk: The chapter could imply that productive agents are literally quantum-entangled or that the Demski result has been rederived here.

Guardrail: Present as organizational analogue. Say measurement can preserve or discard information about joint output; do not call synergy quantum entanglement.

Chapter treatment: Keep, but it remains citation-dependent until the 2008 paper is checked.

### A15. Durability Of Double Entry

Type: Speculative implication.

Support: Plausible synthesis from information-property and historical framing.

Risk: "Explains the survival of double entry" is too strong.

Guardrail: Say "offers one information-theoretic explanation" or "helps explain."

Chapter treatment: Keep in the cautious form now used.

## Highest-Priority Reviewer Defenses

1. If a reviewer asks whether the chapter says accounting is quantum, the answer is no. It says double entry is a classical representational language for relational information.
2. If a reviewer asks whether the gate-set result means accounting systems compute quantum algorithms, the answer is no. The result is representational and requires separate amplitude bookkeeping.
3. If a reviewer asks what the channel-capacity result adds beyond magnitudes, the answer is that scale is abstracted away to isolate the information content of classification and articulation.
4. If a reviewer asks why the second account matters in the channel model, the answer is that it preserves distinctions that collapse for an isolated account under the model's signal-equivalence rule.
5. If a reviewer asks whether the organizational implications are proved, the answer is no. They are disciplined analogies motivated by formal nonseparability and by cited agency theory.

## Recommended Coauthor Checks

- Confirm that the 2022 decision/accounting/information equivalence is described accurately and not extended beyond the source.
- Confirm that the Demski et al. (2008) performance-measurement summary is accurate.
- Confirm that the n-account wording matches the intended theorem: distinguish one-account/two-bit capacity from the broader n-bit extension.
- Decide whether "superposition property" and "entanglement property" should remain as named accounting properties or be softened to "superposition analogue" and "entanglement analogue" throughout.
