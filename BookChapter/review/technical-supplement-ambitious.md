# Technical Supplement

Information Processing with Double Entry in the Quantum Era

Rick Antle, Yale University

John Fellingham, Ohio State University

Haijin Lin, University of Houston

Douglas Schroeder, Ohio State University

## Purpose

This supplement records the formal layer behind the chapter. It is not intended to replace the companion source papers. Its purpose is to make the chapter's claims auditable: what is assumed, what is proved in the source papers, what is a representation claim, and what is an interpretive bridge to accounting.

The organizing distinction is simple. Double entry is not claimed to be a physical quantum system. It is treated as a classical notation and information architecture that can represent selected quantum-information structures and that, in the channel-capacity model, preserves distinctions unavailable to isolated accounts.

## S.1 Claim Classes

| Claim class | Meaning | Chapter examples | Required caution |
| --- | --- | --- | --- |
| Established result | A theorem, proposition, or calculation in a source paper or standard quantum-information result | Toffoli plus Hadamard universality; 5/6 classical odd-cycle ceiling | Cite and state assumptions |
| Representation claim | Double-entry notation can encode or display a formal structure | E/A as basis labels; journal entries as transformations | Do not claim physical implementation |
| Interpretive analogy | A formal structure illuminates an accounting or organizational idea | Bell states as models of nonseparable relationships | Say "analogy," "model," or "structural analogue" |
| Speculative implication | A broader inference about accounting research or organizational design | Double entry's durability as relational architecture | Use "helps explain" or "offers one explanation" |

## S.2 Representation Convention

The accounting notation separates basis labels from amplitudes.

- E labels computational basis state 0.
- A labels computational basis state 1.
- Concatenated labels such as EA, AE, and AEA label computational-basis product states.
- Amplitudes, phases, normalization constants, and measurement probabilities are maintained separately.

For a single qubit, a general state is:

psi = alpha E + beta A, with |alpha|^2 + |beta|^2 = 1.

For a two-qubit system, a general state is:

psi = alpha_EE EE + alpha_EA EA + alpha_AE AE + alpha_AA AA.

The account labels identify the basis components. The amplitudes determine interference and measurement probabilities. This is why the chapter repeatedly says the accounting construction is a notation or representation, not a substitute for quantum probability.

## S.3 Product States, Tensor Products, And Bell States

The state space of a composite quantum system is the tensor product of the component state spaces. This is a statement about spaces. It does not mean every state in the composite space factors into a product of component states.

Product basis states can be represented by concatenated account strings:

- EE represents basis state 00.
- EA represents basis state 01.
- AE represents basis state 10.
- AA represents basis state 11.

A two-qubit state is separable only if it can be written as:

(aE + bA)(cE + dA).

Equivalently, the 2-by-2 coefficient matrix has rank one. Bell states are not rank-one states.

For example, the Bell state Phi+ has the form:

Phi+ = (EE + AA) / sqrt(2).

If Phi+ were separable, it could be written as (aE + bA)(cE + dA). Comparing coefficients requires ac = 1/sqrt(2), bd = 1/sqrt(2), ad = 0, and bc = 0. Those conditions cannot all hold. Therefore Phi+ is nonseparable.

This is the formal basis for using Bell states as models of relational information. The information-bearing object is the joint state, not either component alone.

## S.4 Gate Representation And Universality

The quantum-programming source constructs accounting representations of basic gates. The chapter relies on the following limited proposition.

> **Proposition S1: Representational universality.** If the accounting framework can represent the Hadamard gate and the Toffoli gate, and if amplitudes are tracked separately, then the framework can represent a universal quantum gate set. The proposition is representational and does not claim physical quantum computation.

Support:

- Toffoli is universal for classical reversible computation.
- Aharonov (2003) and Shi (2003) establish that Toffoli together with Hadamard gives quantum universality.
- The quantum-programming source supplies accounting constructions for the relevant gates.

Guardrail:

The safe conclusion is not "double entry is a quantum computer." The safe conclusion is that double-entry notation has enough representational vocabulary to describe the primitive transformations from which universal quantum circuits can be built.

## S.5 Channel Capacity Model

The information-property source treats accounting as a communication channel.

Participants and objects:

- Sender: chooses a journal-entry message.
- Receiver: observes the resulting accounting signal.
- Messages: I, X, Z, and XZ.
- Signal criterion: vectors that are scalar multiples are not distinct signals.
- Scale: dollar magnitudes are abstracted away to isolate classification and articulation.

The four messages represent two bits of possible message choice because log2(4) = 2. The question is whether the accounting structure lets the receiver distinguish all four messages.

## S.6 Why One Isolated Account Collapses Signals

Suppose the starting account is A.

| Message | Resulting account signal | Distinction |
| --- | --- | --- |
| I | A | A-type |
| X | E | E-type |
| Z | negative A | Same signal class as A under scalar-multiple equivalence |
| XZ | E | Same signal class as X |

The sender chose among four messages, but the receiver sees only two distinct signal classes. Therefore an isolated account transmits one bit in this model.

The same collapse appears in the other negative cases considered by the source paper:

- one account on one statement;
- two statement rows with one account;
- two accounts on one statement.

The model's result is therefore not a simple "more accounts" story. Capacity changes only when the additional structure preserves relational distinctions.

## S.7 Two-Bit Channel Capacity

> **Proposition S2: Two-bit capacity under articulation.** In the information-property model, one manipulated account can transmit two bits through the message set {I, X, Z, XZ} when the signal is embedded in two linked statement rows with at least two account columns satisfying the articulation identities.

Accounting interpretation:

- The two rows represent linked statement perspectives, such as accrual and cash-flow views.
- Each relevant account column must satisfy the accounting identity and the cash-flow reconciliation identity.
- The manipulated account is read together with an unchanged second account.
- The unchanged second account preserves distinctions that collapse when the manipulated account is observed alone.

The unchanged account is therefore not inert bookkeeping clutter. It is part of the code. It makes articulation information-bearing.

## S.8 N-Account Extension

The one-account/two-bit result and the n-account extension should not be collapsed into one sentence.

> **Proposition S3: N-account scaling.** In the n-account extension, n-bit capacity arises when the expanded message structure is used and the relevant account columns satisfy the accounting identity and cash-flow reconciliation identity.

Guardrail:

Do not state that an n-account structure automatically produces n bits. The model requires the relevant message space and the articulation conditions. The chapter's careful wording distinguishes:

- one account can reach two-bit capacity when embedded in a qualifying articulated structure; and
- an n-account extension can reach n-bit capacity when the expanded message structure and all relevant articulation conditions hold.

## S.9 Odd-Cycle Game

The three-seat odd-cycle game has seats 0, 1, and 2. The referee assigns Alice and Bob either the same seat or adjacent seats. Each player observes only his or her own seat and reports one of two colors. They win if reports match on same-seat assignments and differ on adjacent-seat assignments.

There are six equally likely assignments:

- three same-seat assignments;
- three adjacent-seat assignments.

Classical strategies cannot two-color a three-cycle without failing at least one adjacent edge. Therefore the best classical strategy wins at most five of six cases.

> **Proposition S4: Classical benchmark.** The optimal classical winning probability in the three-seat odd-cycle game is 5/6.

The entangled case changes the measurement relationship. With the Bell-state strategy used in the companion paper:

> **Proposition S5: Entangled advantage.** The winning probability is 1/2 + sqrt(3)/4 = cos^2(pi/12), approximately 0.933.

The companion paper also considers a superposition-without-entanglement case:

> **Proposition S6: Superposition alone is insufficient in this model.** If one qubit is in superposition and the other is in a basis state, without entanglement, the winning probability is 1/2.

The chapter uses these three cases to support a narrow conclusion: in this coordination problem, the useful resource is the nonseparable relationship, not the mere existence of multiple possible states.

## S.10 Organizational Analogy And Measurement

The performance-measurement section is an analogy, not a quantum theorem. Its purpose is to connect nonseparability to organizational measurement.

The safe claim:

When output depends on a relationship among agents, divisions, or accounts, a measurement system that separates the components may discard information about the joint object. A group or relational measure may preserve information that individual measures suppress.

The unsafe claim:

Productive agents are literally quantum-entangled, or group measurement dominates individual measurement in all settings.

The Demski, Fellingham, Lin, and Schroeder (2008) source should be checked directly before making the agency section carry more than this disciplined analogy.

## S.11 Source Crosswalk

| Chapter claim | Claim class | Principal support | Remaining check |
| --- | --- | --- | --- |
| Double entry is a relational information architecture | Interpretive synthesis | Information-property source; quantum-programming source | Historical durability should remain cautious |
| E/A labels can represent basis states | Representation claim | Quantum-programming source | Keep amplitude caveat |
| Hadamard plus Toffoli gives representational universality | Established result plus representation claim | Aharonov 2003; Shi 2003; quantum-programming source | Do not imply physical implementation |
| One account can transmit two bits only in articulated structure | Established source result | Information-property source | Keep scale abstraction and signal-equivalence rule |
| N-account scaling requires articulation conditions | Established source result | Information-property source | Keep separate from one-account/two-bit result |
| Odd-cycle classical benchmark is 5/6 | Established source result | Odd-cycle source | Explain six assignments |
| Entangled strategy reaches 1/2 + sqrt(3)/4 | Established source result | Odd-cycle source; odd-cycle literature | Restrict to specified strategy/model |
| Superposition without entanglement reaches 1/2 | Established source result | Odd-cycle source | Avoid general anti-superposition language |
| Joint production analogy | Interpretive analogy | Demski et al. 2008; nonseparability idea | Verify source before strengthening |

## S.12 Reviewer-Response Core

If asked whether the chapter claims accounting is quantum:

No. The chapter claims that double entry is a classical relational information architecture that can represent selected quantum-information structures.

If asked whether the universality claim means accounting systems run quantum algorithms:

No. The claim is representational. Physical implementation would require a physical quantum system and coherent amplitude dynamics.

If asked why magnitudes are abstracted away in the channel-capacity model:

The abstraction isolates the information contribution of classification and articulation. It asks what the structure itself can transmit once scale is held constant.

If asked why the second account matters:

The model's signal criterion collapses scalar multiples. The second articulated account preserves distinctions that a single account merges.

If asked whether the organizational implications are proved:

No. They are disciplined analogies supported by the formal examples and by cited agency theory. They should be read as a research direction, not as a theorem.

## References

Aharonov, Dorit. 2003. "A simple proof that Toffoli and Hadamard are quantum universal." arXiv:quant-ph/0301040.

Antle, Rick, John Fellingham, Haijin Lin, and Douglas Schroeder. 2026a. "The channel capacity of the double-entry system." Working paper.

Antle, Rick, John Fellingham, Haijin Lin, and Douglas Schroeder. 2026b. "Double-entry accounting, entanglement, and odd-cycle game." Working paper.

Demski, Joel, John Fellingham, Haijin Lin, and Douglas Schroeder. 2008. "Interaction between productivity and measurement." Journal of Management Accounting Research 20: 169-190.

Fellingham, John, Haijin Lin, and Douglas Schroeder. 2025. "Using double-entry accounting to program quantum computers." Working paper.

Nielsen, Michael A., and Isaac L. Chuang. 2000. Quantum Computation and Quantum Information. Cambridge University Press.

Shi, Yaoyun. 2003. "Both Toffoli and Controlled-NOT need little help to do universal quantum computing." Quantum Information & Computation 3 (1): 84-92.
