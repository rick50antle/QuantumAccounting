# Extracted text: Quantum Programming January 19 2026.docx

Source path: /Users/ra1/QuantumAccounting/BookChapter/sources/Quantum Programming January 19 2026.docx

## Document Body

Using Double-Entry Accounting to Program Quantum Computers

John Fellingham

Fisher College of Business

Ohio State University

Fellingham.1@osu.edu

Haijin Lin

C. T. Bauer College of Business

University of Houston

haijinlin@uh.edu

Douglas Schroeder

Fisher College of Business

Ohio State University

Schroeder.9@osu.edu

January 2026

Abstract

This paper exploits the inherent symmetry and balance of the double-entry accounting system to develop a framework that elucidates the postulates of quantum computing. By representing quantum states with T-accounts and modeling quantum operations through journal entries, we construct the fundamental quantum gates that serve as the building blocks of quantum computers. In particular, we construct the Toffoli gate—a key reversible gate that distinguishes quantum from classical computation—using T-accounts and journal entries. The Toffoli gate is universal for classical computation and, together with the Hadamard gate, forms a universal gate set for quantum computation. Our result demonstrates that the double-entry system functions as a robust information processing mechanism. The proposed double-entry framework offers insights into quantum circuit design and makes quantum computations more accessible to academics and practitioners in business schools.

Keywords: double-entry system, qubit, Toffoli gate, quantum computing, accounting information processing

Introduction

The double-entry system of accounting has endured for over five centuries. In those five centuries, commerce and technology have changed in enormous and unpredictable ways. Nonetheless, the double-entry system has remained remarkably stable and resilient. We might infer, therefore, that there exists a particularly profound or strong property of the double-entry system allowing for this longevity. In this paper, we search for and explore the strength of the double-entry system. In doing so we do not examine how double-entry accounting has been used in the past. Rather we examine its capabilities and imagine what it might be used for.

Historically the double-entry system has served as the mechanism for documenting economic events. We propose extending its use in an information-processing framework. The question is how much could be accomplished if the double-entry system is used for acquiring, processing and communicating information. The answer is that, in the information frame, the double-entry system can actually accomplish quite a bit. In particular, we demonstrate that the logic and structure of double-entry system can model quantum information operations. A rudimentary knowledge of T-accounts and journal entries is sufficient to write programs for quantum computers.

Quantum computers are constructed using the physical operations of the very small, where the laws of physics work differently from our experience in the macro world. Their power lies in the manipulation of quantum bits, or qubits, which—unlike classical bits that are strictly constrained to binary states 0 and 1—can exist in multiple states simultaneously. This new quantum logic enables parallel information processing and achieves significant gains in speed and efficiency for at least some important problems in computer science. Quantum computers are, of course, a relatively recent scientific development.

Remarkably, the ancient double-entry construction can serve as a conceptual language for quantum programs. The double-entry system consists of two components: T-accounts and journal entries. The input to a quantum program is an initial set of T-account balances; the program execution is to apply a sequence of journal entries which maintain the balancing property of the set of T-accounts, and the output is a transformed set of T-account balances. In the basic structure, two types of T-accounts represent two fundamental basis vectors of a qubit, while journal entries represent the bit-flip (X) gate, the phase-flip (Z) gate, and the phase-shift gates such as S and T. Furthermore, we provide the accounting representations for superposition, the Hadamard gate, and the tensor product (allowing composition of multi-qubit systems). The Toffoli gate—a three-qubit reversible gate—is important both as a universal gate for classical reversible computation and as a building block in some quantum error-correction constructions. Using the accounting representation, we are able to show how the Toffoli gate works step-by-step.

The Toffoli gate and the Hadamard gate combined form a universal gate set for quantum computation, meaning that any quantum algorithm can be implemented using circuits composed only of Hadamard and Toffoli gates (Shi 2003; Aharonov 2003). Moreover, Nielsen and Chuang (2000) present four postulates as the core principles for quantum information and computation. In this paper, we provide the accounting representations for each of these four postulates, the state space postulate, the evolution postulate, the composition of systems postulate, and the measurement postulate. It is reasonable to say that the double-entry system provides a coherent representation capable of modeling the acquisition, transformation, and communication of quantum information.

Our attempt aligns with a long tradition of interpretating double-entry system as a rigorous logical system (Paton 1917; Littleton 1928; Ijiri 1989; Arya et al 2000). Cayley (1894) stated, “The Principles of Book-keeping by Double Entry constitute a theory which is mathematically by no means uninteresting: it is in fact like Euclid’s theory of ratios an absolutely perfect one.” Cayley’s interests in double-entry bookkeeping highlights the symmetry and balance embedded in the core principle that every transaction is recorded with two equal and opposite entries so that accounting identity must hold at any point in time. Just as the theory of ratio provides a rigorous foundation for dealing with proportions without relying on the concept of real numbers, the double-entry system provides a logical structure for information processing regardless of the complexity of business development. Viewed through this lens, the double-entry system is connected to the transformation matrices in quantum information theory so that the quantum circuits can be represented in a simple accounting notation.

One contribution of this exercise is that our accounting representation makes the quantum computations much more accessible to academics and practitioners in business schools. It is also plausible that the ability to program quantum computers possesses a certain vocational interest for people familiar with double-entry accounting. Yet the conceptual connection extends beyond pedagogical or vocational considerations. Lloyd (2006) proposed that the universe itself may be understood as a quantum computer, in which information serves as the fundamental unit of physical reality. Perhaps without excessive exaggeration, the double-entry system can be viewed, not only as the language of quantum computers, but also as the language of the universe itself, an entity even older than the double-entry system.

The remainder of the paper is organized as follows. Section II develops the basic structure of the accounting representation for qubit states and single-qubit quantum operations, including the X, Z, T and S gates. We show that the T-accounts exhibit properties analogous to qubits, and that two types of journal entries--reclassification and revaluation entries—correspond to bit flips and phase shifts, respectively. The core structure of this double-entry framework is summarized in a diagram that mirrors the unit circle in the complex plane. Section III extends the framework to more complex quantum operations, including superposition, the Hadamard gate, controlled operations, and the tensor product. Section IV provides the accounting representation of the Toffoli gate. Concluding remarks are provided in Section V.

Basic Structure

Quantum programs and quantum computations are built on a mathematical and conceptual framework governed by four fundamental postulates (Nielsen and Chuang 2000). We aim to provide accounting representations for all four postulates: two in this section and the other two in the next section.

2.1 Qubit states – T-accounts

The fundamental units manipulated by quantum programs are qubits. A qubit can exist in one of two basis states, and , or in any combination of these states.

Postulate 1 (State vector postulate) A qubit is a system represented by a vector in a two-dimensional complex Hilbert space. The two basis states of a qubit are and , analogous to the classical bits 0 and 1.

The basis states of a qubit are represented by T-accounts. The T-accounts work the regular way with debits on the left and credits on the right. For example, an account with 3 on the debit side and 2 on the credit side has a debit balance of 1.

Definition 1 (Accounting representation of qubit states) Define the two basis states of a qubit by two accounts. The account “E” represents state and the account “A” represents state .

It suffices to use two types of accounts to represent the two basis states. Any single-qubit state can be expressed as a linear combination of these two basis states, with complex amplitudes serving as weights that determine the probabilities of measurement outcomes. Furthermore, a quantum gate performed on a qubit is fully determined by how the quantum gate acts on the two basis states.

Quantum Operations – X, Z, S and T

The fundamental single-qubit operations are unitary matrices, meaning the operations preserve the length of the qubits and are invertible. For closed quantum systems (without measurement or decoherence), unitary operations remain fully reversible, meaning one can always undo them to recover the original state. Thus, quantum information stays perfectly preserved, neither created nor lost, throughout the process.

Postulate 2 (Evolution postulate) The evolution of a closed quantum system is described by a unitary transformation.

Unitary operations can be represented using journal entries. It suffices to provide accounting representations for a small set of unitary operations—specifically, the X-gate, the Z-gate, and the T-gate. All the other single-qubit unitary operations, including the S-gate, can be constructed from these quantum gates.

Definition 2 (Accounting representation of the X-gate) The X-gate is a bit flip operation that transforms to , and to . Reclassification entries are used to represent the X-gate, moving amounts between E and A.

In a simple accounting notation, , and . The inverse of X is X.

Definition 3 (Accounting representation of the Z-gate) The Z-gate is a phase flip operation that leaves invariant and changes to . Revaluation entries for an amount of 2 are used to represent the Z-gate, adjusting the balance of A from a debit balance of 1 to a credit balance of 1, and vice versa.

Let denote the T-account with 1 on the debit and 2 on the credit representing . In a simple accounting notation, , and . Similarly, . The inverse of Z is Z.

In Definition 3, the account with 3 on the debit and 2 on the credit can be rescaled by subtracting 2 on both sides and becomes A (the account with 1 on the debit and 0 on the credit). This is the only scaling we require in our representation framework. The Z-gate applies a phase rotation of radians to the state, whereas the T-gate applies a phase rotation of radians. Consistently, the amount of the revaluation entry for the T-gate should be one quarter of the entry for the Z-gate.

Definition 4 (Accounting representation of the T-gate) The T-gate is a phase-shift operation that leaves invariant and changes to . Revaluation entries for an amount of ½ are used to represent the T-gate, adjusting the account balance by ½.

Let denote the T-account with 1 on the debit and ½ on the credit, and denote the T-account with 3/2 on the debit and 2 on the credit. In a simple accounting notation, , and . Similarly, . The inverse of T is represented by the reverse revaluation entries (denoted by ) with an amount of ½. .

Applying the T-gate four times changes to , and vice versa. In the accounting representation, applying the T-entry (Debit Gains/Losses Credit A by ½) four times changes A to .

Applying the T-entry (Debit A Credit Gains/Losses by ½) four times changes to A.

Let denote the T-account with 1 on the debit and k/2 on the credit, and denote the T-account with (2+k)/2 on the debit and 2 on the credit for k=1, 2, 3. In a simple accounting notation, , and . Applying the T-gate four times is equivalent to one Z-gate.

It is possible to construct other quantum operators. For example, applying the T-gate twice is equivalent to one S-gate. Applying the S-gate twice is equivalent to one Z-gate.

Definition 5 (Accounting representation of the S-gate) The S-gate is a phase-shift operation that leaves invariant and changes to . Revaluation entries for an amount of 1 are used to represent the S-gate, adjusting the account balance by 1. In a simple accounting notation, , and . Similarly, . The inverse of S is represented by the reverse revaluation entries (denoted by ) with an amount of 1. .

In sum, all the accounts and for k=1, 2, 3, 4 can be arranged on a circle, called the A circle in Figure 1. The revaluation entries (Z, T, and S) move counterclockwise along the circle, while the corresponding reverse entries (Z, , and ) move clockwise. The A circle mirrors the structure of the unit circle in a complex plane.

Figure 1. The A Circle that mirrors the unit circle

An Accounting Interpretation

The T-accounts and the journal entries in Figure 1 are discussed in a generic form. In this section, we provide one possible interpretation. The two types of accounts are interpreted as flow accounts (accounts with E on the top) and stock accounts (accounts with A on the top). The stock accounts can be revalued and the flow accounts cannot. Reclassification entries transfer dollar amounts from a stock account to a flow account (e.g., depreciating an asset) or from a flow account to a stock account (e.g., capitalizing an expenditure that was initially recorded as an expense).

Revaluation entries are used to revalue the stock accounts downwards. In the A circle of Figure 1, the revaluation entries move accounts counterclockwise. For the accounts on the top half of the A circle, the downward revaluation entries increase the credit side of the stock accounts (for an amount of 2, 1, or ½); therefore, these accounts can be interpretated as assets. In contrast, for the accounts at the bottom half of the A circle, the downward revaluation entries increase the debit side of the stock accounts (for an amount of 2, 1, or ½); therefore, these accounts can be interpreted as liabilities. For example, the stock account with a debit of 1 and a credit of 2 (the account ) has a net credit balance of 1; and therefore, can be treated as a negative asset account or a Liability account. The reverse revaluation entries are to revalue the stock accounts upwards; and thus, move accounts clockwise.

The information in the Gains/Losses account is necessarily embedded in the asset or liability accounts. That is, it is possible to recover the Gains/Losses account balance by examining the asset or liability account; so, for programming purposes, it is not necessary to keep track of the Gains/Losses account balance.

The A circle formulation is not restrictive in two important aspects. First, new accounts can be placed on the A circle using revaluation entries of varying amounts. A phase rotation by radians can be achieved through a revaluation entry of amount ; thereby adding new accounts to the A circle. Second, any transformation from one account to another on the A circle can be realized through an appropriate sequence of journal entries. However, when an operator transforms an account from the top half of the circle to one on the bottom, or vice versa, a single journal entry may not be sufficient to implement the transformation. In such cases, multiple journal entries would be necessary.

Figure 2. An example of using two T-entries to represent one S-entry

To further clarify the second aspect, consider as depicted in Figure 2. This transformation can be implemented using two entries: (i) Debit Gains/Losses Credit A by ½; and (ii) Debit Credit Gains/Losses by ½. Effectively, is achieved by . Nevertheless, for the purpose of describing quantum program, it is sufficient to adopt the accounting notation .

2.4 The E Circle

It is instructive to construct a corresponding E circle by replacing the As on the A circle with Es (shown as the circle on the right-hand-side in Figure 3). Unlike the A circle, the E circle does not contain any arrows, as the accounts on the E circle are not revalued. Any transformation between two accounts on the E circle must be preceded by an X-gate, which moves the account from the E circle to the A circle. After performing the revaluation operations on the A circle, a second X-gate is applied to move the account from the A circle back to the E circle. For example, transforming into could be achieved in three steps: (i) , (ii) , and (iii) . Each step is a journal entry.

In sum, the A circle and the E circle are constructed using the elements of the double-entry system. Any transformation between two accounts can be represented in journal entries. The diagram in Figure 3 offers the double-entry framework for programming quantum circuits, which is the primary focus of this paper.

Figure 3. A visual representation of the double-entry framework

III. More advanced structures

In this section, we extend the double-entry framework in Section II to more complex concepts and operations required for the formulation of quantum circuits.

3.1 Tensor product and conditional operations

Any non-trivial computer program operates on multiple objects (i.e., multiple qubits). In quantum computing, multiple qubits are combined using tensor product, which forms the joint state space of the composite system.

Postulate 3 (Composite system postulate) The state of a composite system is the tensor product of the states of the component systems.

Definition 6 (Accounting representation of the states for composite systems) For a composite system with multiple qubits, its state is the tensor product of the basis states of the individual qubits. The tensor product of the individual qubit states is represented as for .

Applying Definition 6, the state of a two-qubit system is written as EA. The state of a three-qubit system is written as EAE. In a composite system (a system with multiple T-accounts), it is possible to specify conditional operations—that is, conduct an operation on one account conditional on the type of another account.

Definition 7 (Accounting representation of conditional operation) In a composite system, one account serves as the control account and another as the target account. An operator is applied to the target account if, and only if, the control account is on the A circle.

A conditional X-gate on a two-qubit system is written as , the subscript i representing the control account and j the target account. This is also known as the Controlled-NOT (CNOT) gate. For example, the CNOT gate changing into is written as , meaning that given the first account is A, perform the X-gate on the second account and change it from A to E. Similarly, . If the control account is on the E circle, do not perform the operator. That is, . With more than two accounts, we can write the conditional operation in a similar fashion. For example, and are to perform X-gate on the third account conditional on the first account and the second account, respectively.

The Z-gate, the S-gate, and the T-gate can also be applied conditionally. If the control account is on the A circle, perform the operator on the target account. Recall these operators do not change any account on the E circle. For example, , ; and .

3.2 Superposition and the Hadamard Gate

Superposition is one of the most fundamental principles in quantum mechanics. It allows a qubit to exist in the state , the state , or a linear combination of both states. A standard way to create a perfectly balanced superposition from classical bits is the Hadamard gate. For example, a state is a superposition of the two basis states with amplitude for and for . Figure 4 combines Definitions 2 and 3 and illustrates the effect of the H-gate.

Figure 4. Applying the H-gate to one T-account

The second diagram of Figure 4 illustrates , applying H to A is to simultaneously apply X-gate (changing A into E) and to apply Z-gate (changing A into ). One account A is changed into a combination of two accounts, E and , a superposition. This state can be represented using an accounting notation as while the amplitude is recorded separately and used to compute probabilities when a measurement is performed. Because of linearity, the order how the X-gate and the Z-gate are applied (in terms of which operator is on the first row) is not important. Without loss of generality, we put E or on the top row and A or at the bottom row.

Definition 8 (Accounting representation of superposition) A superposition state is a linear combination of the basis states and , represented by , where is on the E circle and on the A circle.

Simply put, the Hadamard gate (or the H-gate) is the normalized sum of the X-gate and the Z-gate. In matrix form, is written as the normalized sum of and , which is . Because both the X-gate and the Z-gate are their own inverses, the H-gate is its own inverse.

Definition 9 (Accounting representation of the Hadamard gate) In a simple accounting notation,

is written as

is written as

is written as

is written as

The inverse of H is H.

When the H-gate is operated on one of multiple accounts, the others are unchanged and go along for the ride. For example, is to apply the H-gate on the first account and is to apply the H-gate on the second account.

Putting accounts into superposition is an extremely useful programming tool as both rows can be processed simultaneously (known as quantum parallelism in Nielsen and Chuang (2000)). For example, represents a quantum program that operates on two qubits (accounts). First, apply the H-gate to the first qubit to create a superposition; then, apply the X-gate to the second qubit in each row conditional on the first qubit on the A circle.

We can also extend this process to a system with more than two qubits (accounts). An example with three accounts is illustrative as follows.

The first operator is to create a superposition of the first qubit, ; the second operator is to perform a conditional X-gate on the second qubit of each row while using the first qubit as the control qubit; the third operator is to perform a conditional X-gate on the third account of each row while using the second qubit as the control qubit; and the fourth operator is to revalue the first qubit of each row.

3.3 Recomposition operation

There are simplifications in quantum computations. In particular, the fractional revaluations (phase shift operations the T-gate and the S-gate) can be loaded entirely on the last qubit (i.e., last account) so that there is only one fraction to deal with. This can be achieved using the journal entries that involve the two accounts. Collectively, we call these journal entries as recomposition entries.

Definition 10 (A recomposition entry) A recomposition entry transforms “” into “,” or vice versa, for any .

To understand Definition 10, consider an example where is changed into . The recomposition entry is recorded as Debit First Account Credit Second Account by ½.

In contrast to the journal entries, X, Z, S and T, that perform the information processing activities, the recomposition entries do not change the information properties of the T-accounts.

To perform an operation and shift fraction to the last qubit, it is straightforward to take three steps. The first step is to implement a recomposition entry to move the phase to the qubit that needs to be transformed; the second step is to perform the transformation; and the third step is to implement a recomposition entry to move the fraction phase to the last qubit. For example, can be implemented in the following steps.

Step 1: Change into using a recomposition entry, Debit Third Account Credit Second Account by 1.

Step 2: Perform to change into .

Step 3: Change into using a recomposition entry, Debit Second Account Credit Third Account by ½.

3.4 Measurement

When a closed quantum system is observed (measured), the system is instantly changed. Before any measurement, the state of the system is in a superposition of all possible outcomes (a linear combination of basis states with complex amplitudes); and the probability of each outcome is the squared magnitude of the amplitude. Upon measurement, the system state collapses to the state corresponding to the observed outcome. For example, consider a single-qubit system in a state . When we measure the qubit, the post-measurement state might be a or a . The probability of the state is and the probability of state is .

Postulate 4 (Measurement postulate) Quantum measurements are described by a collection of measurement operators. The index m refers to the measurement outcomes. If the state of the quantum system is before measurement, the probability that result m occurs is .

Definition 11 (Accounting representation of measurement) Let E and A be the computational basis for a single qubit. Let EE, EA, AE, and AA be the two-qubit computational basis. Let a combination of E and/or A be the multiple-qubit computational basis. The amplitudes are recorded separately. Measurement collapses to one basis state with the probability as the squared magnitude of the amplitude for the basis state.

Measurement is not the focus of this paper. We will explore the application of the measurement postulate in future studies.

IV. The Toffoli Gate

In this section, we use T-accounts and journal entries to program the Toffoli gate. The Toffoli gate is universal for classical computation and can also be implemented as a quantum logic gate (Nielsen and Chuang 2000, p. 188). As a result, quantum computers subsume classical computers in the sense that any computation achievable on a classical computer can also be implemented on a quantum computer. Moreover, Shi (2003) and Aharonov (2003) proved that the Toffoli gate combined with the Hadamard gate forms a universal gate set for quantum computation. For these reasons, this section focuses on the Toffoli gate.

Table 1. Accounting representation of the truth table for the Toffoli gate

| Input | Output |
| --- | --- |
| EEE | EEE |
| EEA | EEA |
| EAE | EAE |
| EAA | EAA |
| AEE | AEE |
| AEA | AEA |
| AAE | AAA |
| AAA | AAE |

The Toffoli gate is a three-qubit operator with two control qubits and one target qubit. It flips the target qubit if, and only if, the first wo qubits are both in the state . Table 1 lists all eight possible input states and their corresponding outputs using the accounting notation. As shown in the last two rows, when the first two accounts are both A, the third account is flipped from A to E or from E to A. In the first six rows, the output is identical to the input. Every input state produces a distinct output, so no information is lost.

The Toffoli gate can simulate many classical logical gates. However, classical logical gates are inherently irreversible. For example, the NAND (NOT-AND) gate outputs 0 if, and only if, all of the inputs are 1, and outputs 1 otherwise. Table 2 shows the truth table for a three-input NAND gate. Although there are eight possible input combinations, there are only two possible outputs (0 or 1). Because different inputs lead to the same output, the input cannot be uniquely recovered from the output. As a result, information is unavoidably lost.

Reversibility is one reason quantum computers are superior to classical computers. Because all quantum operations are unitary and thus reversible, each output state uniquely determines its input state. This one-to-one mapping guarantees the conservation of information throughout the computation process. In contrast, the classical operations inevitably discard information by mapping multiple inputs to the same output. According to the Landauer’s principle, energy is expended (and heat is generated) when information is erased (Nielsen and Chuang 2000, p. 153). The reversibility of the quantum operations (equivalently, the reversibility of journal entries) ensures the conservation of information, and hence, avoids the associated expenditure of energy.

Table 2. The truth table for the NAND gate with three inputs

| Input a | Input b | Input c | Output |
| --- | --- | --- | --- |
| 0 | 0 | 0 | 1 |
| 0 | 0 | 1 | 1 |
| 0 | 1 | 0 | 1 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 0 | 1 |
| 1 | 0 | 1 | 1 |
| 1 | 1 | 0 | 1 |
| 1 | 1 | 1 | 0 |

Accounting representation of the Toffoli gate

The decomposition of the Toffoli gate is written as follows.

Toffoli Gate

We use the accounting notation to illustrate the operation of the Toffoli gate step by step. Suppose the input to the program is AEA. According to Table 1, the output is also AEA, written in a simple accounting notation as , indicating that no conditional bit flip occurs. The A circle and the E circle (in Figure 3) are useful for tracking the effects of the S, T and Z operations. The recomposition operation is applied wherever needed.

As another example, if the input is AAE, a bit flip occurs on the third qubit. In a simple accounting notation, this transformation is written as .

The accounting representation offers intuition for how the Toffoli gate is implemented. (i) When the target qubit is initially in either state or state , the first operator creates a superposition on the target qubit. (ii) The sequence forms the core of the Toffoli gate and flips the target qubit if, and only if, both control qubits are in the state . (iii) The sequence {} temporarily changes the two control qubits from AA to AE. (iv) The second operator removes the superposition on the target qubit. (v) The next sequence {} restores the two control qubits from AE back to AA. (vi) Lastly, the sequence {} performs cleanup operations on the control qubits to eliminate the trailing fractions.

Concluding Remarks

The elegance of the double-entry system is embodied in a few ideas which can be presented in one or two introductory accounting lectures. This paper emphasizes two such ideas: (i) how T-accounts work, and (ii) how journal entries connect T-accounts. We discuss the similarity between the double-entry objects, T-accounts, and quantum objects as well as the double-entry operations, journal entries, and quantum operations.

Although our focus is on information processing, the two important types of journal entries are recognizable in the economic event documentation frame. First, reclassification (X) changes back and forth between account A and account E. Second, revaluation (Z, T, and S) is performed on account A but not on account E. The heavy lifting of information processing is carried out by X, Z, S, T, and the Hadamard gate (a simple combination of X and Z).

The question is how powerful these double-entry tools are for information processing. The answer is that they are quite powerful, as illustrated by their ability to represent all four postulates in quantum computations. We have accomplished the construction of quantum programs using T-accounts and journal entries. In particular, we provided an accounting representation of the Toffoli gate, which is universal for classical computation.

The accounting representation of the Toffoli gate conveys four key ideas. First, it illustrates a concrete double-entry construction for a specific quantum program. Second, because the Toffoli gate is universal for classical computation, the double-entry framework extends naturally to represent any classical computer program. Third, because the Toffoli gate, combined with the Hadamard gate, forms a universal gate set for quantum computation, the double-entry framework can be generalized to represent any quantum program. Fourth, the double-entry framework highlights a fundamental advantage of quantum computing—reversibility—which is intrinsic to quantum computing but cannot be fully achieved in classical computing. Reversible computation reduces energy consumption.

Although our original intent was to explore other possible ways to use the power of the double-entry system, this study has yielded broader insights about the double-entry system. Since we can use T-accounts and journal entries to program quantum computers, and since reversibility is one key reason quantum computers are superior to classical computers, it is not too farfetched to speculate that reversibility is one key reason why double-entry systems are superior to single-entry system for information processing.

There might be additional reasons why double-entry systems outperform single-entry systems. For example, quantum computers can exploit the power of entanglement. It is conceivable that analogous mechanisms might exist within the double-entry system. But such possibilities remain speculative and are left for future research.

References

Anil, A., J. C. Fellingham, J. C. Glover, D. A. Schroeder, and G. Strang. Fall 2000. “Inferring transactions from financial statements,” Contemporary Accounting Research Vol. 17 (3): 365-385.

Antle, R., Fellingham, J., H. Lin, and D. Schroeder. 2025. An Information Property of Double Entry Accounting. Working paper.

Aharonov, Dorit. 2003. “A simple proof that Toffoli and Hadamard are quantum universal,” arXiv:quant-ph/0301040.

Cayley, A. 1894. The Principles of Book-Keeping by Double Entry. Cambridge: At the University Press. London: C. J. Clay and Sons.

Fellingham, J., H. Lin, and D. Schroeder. 2022. Entropy, Double Entry Accounting and Quantum Entanglement. Foundations and Trends in Accounting 16 (4): 308-396.

Ijiri, Yuji. 1989. Momentum Accounting and Triple-Entry Bookkeeping: Exploring the Dynamic Structure of Accounting Measurement. American Accounting Association, Sarasota, Florida.

Littleton, A. C. June 1928. “Paciolo and modern accounting,” The Accounting Review Vol. 3 (2), p131-140.

Lloyd, S. 2006. Programming The Universe: A Quantum Computer Scientist Takes on the Cosmos. Vintage Books, A Division of Random House, Inc., New York.

Nielsen, M. A. and I. L. Chuang. 2000. Quantum Computation and Quantum Information. Cambridge University Press.

Paton, W. A. 1917. “Theory of the double-entry system,” Journal of Accountancy Vol. 23 (1): p7-26.

Pelaez, Emilio. 2021. “A clever quantum trick.” Quantum Untangled (Medium), January 16, 2021. https://medium.com/quantum-untangled/a-clever-quantum-trick-54f27e2518a4

Shi, Y. 2003. “Both Toffoli and controlled-Not need little help to do universal quantum computing,” Quantum Information & Computation 3(1): 84-92.

## Footnotes

- footnote 1: Fellingham et al. (2022) demonstrates the equivalence of three frames, decision, accounting and information frames, in a generic setting where a Kelly investor repeatedly makes bets to maximize terminal wealth. Maximizing terminal wealth is equivalent to maximizing the expected return for each round (this is the decision frame). The expected return equals the logarithm of one plus accounting return under geometric mean accounting valuation (this is the accounting frame). The increase of expected return due to information equals mutual information, which is the reduction of entropy due to information (this is the information frame). Under the information frame, it is not necessary to specify the economic context while studying the double-entry system as an information processing mechanism.
- footnote 2: Quantum computing relies on a set of fundamental operators (also called gates) that operate on quantum states. Quantum gates are always represented by unitary matrices, which means they are reversible, preserve state norms, and form the mathematical backbone of quantum circuits for quantum algorithm execution. In this paper, we are able to merely use T-accounts and journal entries to represent these operators and the quantum algorithms.
- footnote 3: As defined in Nielsen and Chuang (2000, p. 188), “… a set of gates is said to be universal for quantum computation if any unitary operation may be approximated to arbitrary accuracy by a quantum circuit involving only those gates.” Aharonov (2003) stated that the Toffoli gate alone is sufficient to perform all classical reversible computations, and further argued that the Hadamard gate and the Toffoli gate together constitute the simplest and most natural universal set of gates one could hope for.
- footnote 4: As Lloyd (2006) stated, “The universe is the biggest thing there is and the bit is the smallest possible chunk of information. The universe is made of bits. Every molecule, atom, and elementary particle register bits of information. Every interaction between those pieces of the universe processes that information by altering those bits. … Because the universe is governed by the laws of quantum mechanics, it computes in an intrinsically quantum-mechanical fashion; its bits are quantum bits. The history of the universe is, in effect, a huge and ongoing quantum computations. The universe is a quantum computer. … The universe computes its own behavior. (pages 3-4)”
- footnote 5: This is a simplified version of Postulate 1 in Nielsen and Chuang (2000, p. 80). It is natural and practical to start with a single qubit.
- footnote 6: As discussed later in the measurement postulate, the amplitudes can be recorded separately. The computation of probabilities from using these amplitudes is beyond the scope of this paper.
- footnote 7: There are two key properties of unitary operators U: (i) they are invertible, meaning the inverse is the adjoint matrix, ; and (ii) they preserve norms, for any state vector x. In contrast to classical computing, most quantum operations are unitary; these two properties imply that unitary operations are reversible. A reversible operation guarantees that the initial state can be uniquely recovered from the final state, ensuring that no information is lost during the operation and thus preserving the conservation of information.
- footnote 8: In matrix form, .
- footnote 9: It is helpful to interpret the Z-entry (i.e., the Z-gate) as adding a “hat.” Applying the Z-entry to yields , that is, ; An account with two “hats” can be scaled back to A.
- footnote 10: The A circle in Figure 1 corresponds to a unit circle in the complex plane containing eight evenly spaced points, with and serving as the endpoints of the horizontal diameter. Adjacent points are separated by radians. Each point on the circle can be expressed in the form , using Euler’s formula.
- footnote 11: For example, if an asset account changes from a beginning debit balance of 1 to an ending credit balance of 1, the asset decreases by 2, and the corresponding entry must be a debit of 2 to the Gains/Losses account.
- footnote 12: Noted that a single journal entry—Debit Gains/Losses Credit A by 1—would not be sufficient. Although subtle, this distinction does not undermine the central claim that any transformation between two accounts on the A circle can be implemented through an appropriate sequence of journal entries.
- footnote 13: Postulate 3 here is Postulate 4 in Nielsen and Chuang (2000, p. 94).
- footnote 14: The CNOT gate is a fundamental operation on two qubits. One qubit is a control qubit and the other qubit is a target qubit. If the control qubit is |0>, the target qubit remains unchanged. If the control qubit is |1>, the target qubit flips.
- footnote 15: Intuitively, applying the H-gate twice results in the same output as the initial input. It is easy to see using the accounting notation. For example, consider the initial state is E. Applying the H-gate twice is written as follows. The first H-gate changes E to . The second H-gate applied to E and A separately results in the output including E, A and . Noted that the accounts A and have a net balance of zero—so they effectively cancel each other out. As a result, the only remaining output is E; implies that the H-gate is its own inverse.
- footnote 16: This is the process of creating a Bell state, in particular, the state . In matrix form, is written as the normalized sum of and , resulting in . One interesting feature about the Bell states is that they are entangled. Entanglement is not the focus of this study. Fellingham et al. (2025) provides more detailed discussions on this topic.
- footnote 17: In matrix form, the initial state is . The first operator is an 8 x 8 matrix given by is the n x n identity matrix. After applying this operator, the state becomes . The second operator is , where denotes the n x n zero matrix and . After this operation, the state is The third operator is , which transforms the state into . Finally, the last operator is , resulting in the final state . To confirm the accounting notation, is the normalized sum of and , corresponding exactly to as obtained above.
- footnote 18: All fourteen entries are available from the authors upon request.
- footnote 19: In accounting, we sometimes make adjusting entries to move amounts from one account to another (e.g., the closing entries to move amounts from the revenue account and the expense accounts to Income summary). The recomposition entries are similar to these adjusting entries.
- footnote 20: This essentially is phase kickback in quantum computing (Pelaez 2021). Phase kickback is a very common and useful trick that is applied in larger quantum algorithms such as Shor’s and Grover’s.
- footnote 21: For clarity, the recomposition entry is explicitly indicated whenever needed. For example, is implemented in the three steps as described.
- footnote 22: Here and are complex amplitudes satisfying .
- footnote 23: This is Postulate 3 in Nielsen and Chuang (2000, p. 84).
- footnote 24: This means that any quantum algorithm can, in principle, be implemented using the circuits composed only of the Toffoli and the Hadamard gates. As the universality set for quantum computers is larger than that for classical computers, it is plausible that quantum computers can do more than classical computers. One capability available to quantum computers, which is not available classically, is reversibility.
- footnote 25: The Toffoli gate, also known as the CCNOT (controlled-controlled-Not) gate, is named after computer scientist Tommaso Toffoli at Boston University. Its reversibility makes the Toffoli gate especially useful in quantum computing and quantum error correction. In contrast to many classical logic gates that irreversibly discard information, computations performed with the Toffoli gate can be undone, thereby preserving all information in the system.
- footnote 26: The Toffoli gate is universal for classical computation because it can simulate the NAND gate and the FANOUT gate. The NAND gate and the FANOUT gate are together universal for classical computation (Nielsen and Chuang 2000, p. 159-160). The NAND gate is the negation of the AND gate; the FANOUT gate is the copying gate.
