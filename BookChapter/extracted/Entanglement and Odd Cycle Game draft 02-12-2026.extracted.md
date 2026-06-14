# Extracted text: Entanglement and Odd Cycle Game draft 02-12-2026.docx

Source path: /Users/ra1/QuantumAccounting/BookChapter/sources/Entanglement and Odd Cycle Game draft 02-12-2026.docx

## Document Body

Double-entry Accounting, Entanglement, and Odd-cycle game

Rick Antle

Yale School of Management

Yale University

rick.antle@yale.edu

John Fellingham

Fisher College of Business

The Ohio State University

Fellingham.1@osu.edu

Haijin Lin

C. T. Bauer College of Business

University of Houston

haijinlin@uh.edu

Douglas Schroeder

Fisher College of Business

The Ohio State University

Schroeder.9@osu.edu

Introduction

The purpose of this paper is to offer one explanation why double-entry system is superior to single-entry system in a simple odd-cycle game with restricted information channel.

The setup

The odd-cycle game provides a setting with a restricted information channel. In this game, a referee randomly chooses a seat assignment for two players, Alice and Bob, around a round table with an odd number of seats. The assignment consists of either the same seat to both players or two adjacent seats with Alice’s seat always to the left of Bob’s seat. Each player knows only their own seat assignment. Before the game starts, Alice and Bob may coordinate and agree on a joint strategy to maximize the probability of winning the game together. After the seats are assigned, the referee then independently asks each player to submit a report. The players win the round if they submit the same report when assigned the same seat, and different reports when assigned adjacent seats. The information channel is restrictive in that the number of possible reports is strictly smaller than the number of seats. Without this restriction—that is, when the number of reports equals the number of seats)—the players can always encode their seat assignments and win with probability one.

Without loss of generality, we consider a round table with three seats labeled . There are six possible seat assignments, written as , where the first digit denotes Alice’s seat and the second denotes Bob’s seat. Each player reports one of two colors, {Red, Blue}.

Table 1. Classical probability of winning under a pure strategy

| Seat assignment | Alice’s report | Bob’s report | Prob(winning) |
| --- | --- | --- | --- |
| 00 | Red | Red | 1 |
| 01 | Red | Blue | 1 |
| 11 | Blue | Blue | 1 |
| 12 | Blue | Red | 1 |
| 22 | Red | Red | 1 |
| 20 | Red | Red | 0 |

Before the game begins, each player chooses a strategy specifying which color to report for each possible seat they might be assigned. A pure strategy therefore assigns a single color to every seat. One example of a pure strategy that achieves the highest probability of winning is for both players to report Red when assigned an even-numbered seat and Blue when assigned an odd-numbered seat, as illustrated in Table 1. This strategy wins for all seat assignments except the last one. When Alice is assigned seat 2 and Bob assigned seat 0, both players report Red, which causes them to lose. Since all six seat assignments are equally likely, the overall probability of winning is therefore 5/6.

Lemma 1 characterizes the optimal solution to the odd-cycle game. As shown in its proof, allowing mixed strategies does not improve the probability of winning beyond what is achievable by pure strategies.

Lemma 1. In a three-seat odd-cycle game, randomization does not provide advantage. There exists a pure classical strategy that attains the optimal winning probability 5/6, and no mixed strategy can do better.

Main analysis

In this section, we show that when quantum strategies are permitted, the probability of winning in the odd-cycle game increases relative to the classical benchmark (as described in Lemma 1). To ensure that these quantum strategies are accessible to readers without requiring much prior background in quantum information, we first briefly introduce the double-entry representation of quantum information processing that is relevant to solve the odd-cycle game, and then properly define the three-seat cycle game (Section 3.1). Next, we characterize the optimal solution to the game and present three results depending on the various initial states of the two players (Section 3.2). Lastly, we compare the optimal outcome under quantum and classical strategies; the comparison in turn sheds lights on the information-processing power of the double-entry system (Section 3.3).

3.1 The double-entry framework of quantum information processing

Fellingham et al. (2026) provide the double-entry representation of the four postulates in quantum information theory (Nielsen and Chuang 2000). In particular, the constructs of the Hadamard gate and the Toffoli gate using accounts and journal entries signify the capability of the double-entry system to simulate any quantum program. In this section, we provide a summary of the accounting representations that are directly relevant to our analysis. These definitions are based on the double-entry framework developed in Fellingham et al. (2026), with terminology and notation customized for the analysis of the odd-cycle game.

A qubit is the fundamental element in quantum computing. It suffices to use two types of accounts to represent the two basis states for a qubit. A quantum operator performs on a qubit is fully determined by how the quantum operator acts on the two basis states.

Definition 1 (Accounting representation of qubit states) A qubit has two basis states, and . The account “E” represents state and the account “A” represents state . Moreover, the account “” represents .

Definition 2 (Accounting representation of quantum gates) Quantum gates are unitary transformations that can be represented by journal entries. The bit flip, the phase flip and the phase shift operators can be used to construct other quantum gates.

The bit flip operator, the X-gate, transforms to , and to . The X-gate is represented by reclassification entries that move amounts between E and A, in simple accounting notation as and .

The phase flip operator, the Z-gate, changes to and leaves invariant. The Z-gate is represented by revaluation entries of amount 2 that adjust the balance of A and do not adjust the balance of E, in simple accounting notation as , , and .

The phase shift operator, the -gate, is represented by revaluation entries of amount that adjust the balance of A and do not adjust the balance of E.

In a simple accounting notation, is represented as , where the notation “” in “” indicates that the amplitude for state is . Moreover, .

Definition 3 (Accounting representation of the Hadamard gate) The Hadamard gate (H-gate) combines the effects of the X-gate and the Z-gate. When applied to a basis state, the H-gate produces a superposition where the qubit is equally likely to be measured as or . In the double-entry representation framework, the H-gate is to apply both the reclassification and the revaluation entries, producing two entries. In simple accounting notation,

is represented as ;

is represented as ;

is represented as ; and

is represented as .

Definition 4 (Accounting representation of two-qubit state) The joint state of two qubits is defined as the tensor product of the basis states of the individual qubits:

, .

The four computational basis states , , , and are represented in simple accounting notation as EE, EA, AA, and AE, respectively.

Definition 5 (Accounting representation of measurement postulate) A quantum system exists in a superposition of basis states until a measurement is performed. Each basis state is associated with a complex probability amplitude, and the probability of measuring a basis state is given by the amplitude multiplied by its complex conjugate. Given the amplitude of a basis state , the probability is .

3.2 The game

In a three-seat cycle game with quantum strategies, there are six possible seat assignments, . Each player is a qubit, and the three-seat cycle game is described as a two-qubit composition system. Each player chooses an action, represented by a phase-shift angle, conditional on its own seat assignment, . The evolution of the system is implemented by a quantum process (defined by a sequence of journal entries), . Measuring the state of this system yields one of four possible outcomes corresponding to the four computational basis states, EE, EA, AE, AA. The two players win under either of the following two cases: (i) they are assigned the same seat and the measured state is EE or AA; or (ii) they are assigned adjacent seats and the measured state is EA or AE.

We consider three cases that differ in the initial states, which characterize the two players. In the first case, neither player is in superposition, and the initial state is represented by AA. In the second case, both players are in superposition and entangled (will be explicitly defined), and the initial state is represented by . In this third case, only one player is in superposition, and the initial state is represented by .

Case 1: two qubits both in basis states

Consider the case in which the two players are represented by two qubits that are both in basis states and combined using tensor product. Without loss of generality, the initial state can be AA. For a given seat assignment, if the first player (Alice) chooses and the second player (Bob) chooses , the initial state then evolves under the quantum process with parameters and .

The measurement yields outcomes in four basis states with probabilities determined by the corresponding amplitude multiplied by its complex conjugate. Recall the notation “” represents the amplitude “” for . To maintain the sum of the probabilities is one, we rescale each probability by 16.

Applying the Euler’s identity, , we can compute the probability of both players obtaining the same measurement outcome and the probability of the two players obtaining different measurement outcomes.

There are six possible seat assignments. The probability of winning can be written as follows.

The optimal strategies that maximize the probability of winning are summarized in Proposition 1.

Proposition 1. In a three-seat odd-cycle game that admits quantum strategies, if neither qubit is in superposition and the initial state is a tensor product of two basis states, the maximum winning probability attainable is 5/6. In particular, quantum strategies do not outperform optimal classical strategies.

Proposition 1 suggests that the odd-cycle game with quantum strategies could simulate the classical game. With the two qubits that are not in superposition, this is the best outcome achievable under quantum strategies.

Case 2: two qubits in superposition and entangled

The two qubits, initially prepared in the basis states, can be entangled by applying two sequential operations: first a Hadamard gate on the first qubit (), and then a controlled X-gate (also known as CNOT gate, denoted by ) which applies the X-gate on the second qubit if and only if the first qubit is either state A or state . For example, applying these operations to EE yields:

The state is entangled because it cannot be written as a tensor product of two single-qubit states. Similar, applying the two operators to the other three basis states yields:

The resulting four states are the Bell states, which are the maximally entangled states of two qubits.

Definition 6 (Accounting representation of the Bell states) The Bell states are the states of two qubits that are maximally entangled. There are four Ball states, in simple accounting notations, written as , , , and .

Consider the case in which the two players are represented by two entangled qubits. Without loss of generality, assume the initial state is . For a given seat assignment, if the first player (Alice) chooses and the second player (Bob) chooses , the initial state then evolves under the quantum process with parameters and .

The probability for each measured state is computed as follows. To maintain the sum of the probabilities is one, we rescale each probability by 32.

Furthermore, we compute the probability of both players obtaining the same measurement outcome and the probability of the two players obtaining different measurement outcomes.

There are six possible seat assignments. The probability of winning can be written as follows.

The optimal strategies that maximize the probability of winning are summarized in Proposition 2.

Proposition 2. In a three-seat odd-cycle game that admits quantum strategies, if the two qubits are entangled, the maximum winning probability attainable is 0.933. This exceeds the optimal classical solution, demonstrating that quantum strategies can strictly outperform classical ones.

Case 3: only one qubit is in superposition

Consider the case in which one player is in a superposition while the other player is in the basis state. Without loss of generality, Alice is in superposition and Bob is not; the initial state is . For a given seat assignment, if the first player (Alice) chooses and the second player (Bob) chooses , the initial state then evolves under the quantum process with parameters and .

The probability for each measured state is computed as follows. To maintain the sum of the probabilities is one, we rescale each probability by 32.

Furthermore, we compute the probability of both players obtaining the same measurement outcome and the probability of the two players obtaining different measurement outcomes.

There are six possible seat assignments. The probability of winning is one half.

Proposition 3. In a three-seat odd-cycle game that admits quantum strategies, if one qubit is in a superposition and the other qubit is in a basis state, the two qubits are not entangled. The maximum winning probability attainable is 0.5. This is strictly below the optimal classical solution, demonstrating that quantum strategies could perform strictly worse than classical ones.

3.3 Accounting interpretation

The ability of the double-entry system to represent the quantum programming indicates that the double-entry system functions as a vector-processing device. In contrast, the single-entry system is a scalar processor. The three-seat cycle game provides a natural setting to assess the information-processing capability under the double-entry system. In this context, the game that admits quantum strategies uses quantum programming to process inputs from the players, and thus, can be treated as a double-entry system. Conversely, the game restricted to classical strategies corresponds to a single-entry system.

The double-entry representation of a superposition (Definition 3) has a two-row structure that can be interpreted as a structure of two financial statements. Under the double-entry system, financial statements articulate as long as two identities hold at every point in time.

Definition 7 (Articulation of financial statements) Under the double-entry system, the following two identities hold at every point in time, guaranteeing the articulation among the financial statements.

The accounting identity, Assets = Equities, prescribes the accrual statement (including the balance sheet and the income statement).

The cash flow reconciliation identity, , reconciles the accrual-based income with the changes in cash, prescribing the statement of cash flows.

The H-gate transforms an initial basis state into a superposition. In accounting terms, the articulation of the financial statements provides a structural analogue of superposition. The superposition property of the double-entry system lies in the articulation of the financial statements.

Definition 8 (Superposition property) The superposition property of the double-entry system is its ability to record information across multiple financial statements while maintaining articulation among the statements. From an information-processing perspective, how information is recorded on one financial statement is not as important as how information is recorded on all financial statements.

To clarify how articulation of financial statements is analogous to superposition, we rewrite the two identities in Definition 7 to reflect the effect of journal entries. The accounting identity holds if the changes of equities equal the change of assets. In particular, Income equals the sum of the changes in cash and the changes in (non-cash) assets:

(1) where denotes the change in non-cash assets. The cash flow reconciliation identity holds if the net changes in Cash equal to Income minus the adjustments:

(2) where denotes total non-cash adjustments (e.g., depreciation or impairment). Adding (1) and (2) yields

(3)

The equality (3) states that changes of non-cash assets equal the non-cash adjustments made to reconcile accrual income to cash. This equality ensures that the accrual statement and the cash flow statement articulate.

Consider a cash purchase of an asset. The asset is recognized on the balance sheet, and the starting point is “A.” A subsequent reclassification entry such as depreciation reduces the balance of the asset and generates a non-cash adjustment in the cash flow statement.

Accounting identity

Cash flow reconciliation identity

Similarly, a subsequent asset impairment entry reduces the balance of the asset and requires a non-cash adjustment in the cash flow statement.

Accounting identity

Cash flow reconciliation identity

Effectively, the accounting process maps changes in the asset into reconciliation adjustments to accrual income. Information about the asset—that is, the economic activities affecting it—is transmitted through reclassification and revaluation entries. The underlying information appears simultaneously across multiple financial statement:

Change in the asset on the balance sheet

Expense or loss in the income statement, and

Non-cash adjustment in the cash flow statement.

Just as a Hadamard gate acting on a basis state produces a superposition state that exists in multiple basis states (in a simple accounting notation, ), the articulation property of the double-entry system ensures that information is processed and presented across multiple financial statements while preserving internal consistency.

The superposition property may hold for one division but not for another. In other words, one division’s information can be processed and transmitted through multiple financial statements, while another division’s information is processed only in one financial statement. This typically occurs when the two divisions are independent and not connected. However, when the two divisions are connected, the superposition in one division suggests that the other division can also process information through multiple financial statements. This interdependence is analogous to the entanglement property of the double-entry system.

Definition 9 (Entanglement property) The entanglement property of the double-entry system is when multiple divisions are connected and information from multiple divisions is jointly processed across multiple financial statements.

Our analyses in Section 3.2 demonstrate that the double-entry system outperforms the single-entry system only when the entanglement property of the double-entry system is at work. That is, if the two divisions are connected and if the information from both divisions is jointly processed through multiple financial statements, the double-entry system is superior to the single-entry system. In contrast, if a division’s information is processed through a single financial statement, the double-entry system offers no advantage over the single-entry system. Moreover, when two divisions are not connected but one or both divisions process information using only one statement, the double-entry system may be outperformed by the single-entry system.

Concluding remarks

To be added later

Reference

Drmota, A., D. Main, E. M. Ainley, A. Agrawal, G. Araneda, D. P. Nadlinger, B. C. Nichol, R. Srinivas, A. Cabello, and D. M. Lucas. 2025. “Experimental quantum advantage in the odd-cycle game.” Physical Review Letters 134, 070201.

Fellingham, J., H. Lin, D. Schroeder. 2026. “Using double-entry accounting to program quantum computers,” working paper.

Nielsen, M. A. and I. L. Chuang. 2000. Quantum Computation and Quantum Information. Cambridge University Press.

Appendix

Proof of Lemma 1.

We begin by analyzing pure strategies in the odd-cycle game with 3 seats. A pure strategy is defined by , where is Alice’s report when assigned seat i, and is Bob’s report when assigned seat i. The solution concept is Nash equilibrium. A strategy in which a player reports the same color for all seat assignments (that is, ) is never optimal. The pure-strategy equilibria can be summarized in two forms: (i) the two players adopt identical (non-constant) reporting strategies, and for some ; and (ii) the two players’ reports differ at exactly one seat and coincide at the remaining two seats, . Under these strategies, the expected probability of winning is 5/6.

Next, we show that a mixed strategy won’t improve over pure strategies. Consider a pure strategy under which Alice adopts strategy RRB (that is, ) and Bob adopts strategy RBB (that is, ). The players lose when both are assigned to seat 1 and the probability of winning is 5/6.

Both players consider a mixed strategy. Alice considers to implement strategy RRB with probability p and RBB with probability (1-p). Bob considers to implement strategy RBB with probability q and RRB with probability (1-q).

The last inequality is implied because . In general, because the probability of winning under any pure strategy is at most 5/6, and because a mixed strategy is a probability distribution over pure strategies, the probability of winning achieved by any mixed strategy is a convex combination of the probabilities achieved by pure strategies. As a result, no mixed strategy can yield a probability of winning exceeding 5/6. Q.E.D

Proof of Proposition 1.

First, applying the definitions in Section 3.1, we are able to represent the quantum operation on the initial state AA.

Note that acts only on the ith qubit for . When an operator is applied to one qubit, the other qubit remains unchanged (i.e., it evolves under the identity operator). For example, when is applied to the initial state AA, it creates a superposition on the first qubit: , while the second qubit remains in state A. To add up the amplitudes for the same basis state, observe that with amplitude , , is equivalent to EA with amplitude ( . Therefore, EA and can be combined by adding their amplitudes, yielding .

Next, for a given seat assignment and the two players’ phase-shift angles, for Alice and for Bob, the probability of obtaining the state EE is computed as:

Applying the Euler’s identity,

Similarly,

The probabilities of getting the same signals and getting different signals are computed, respectively, as follows:

Third, for a seat assignment ij where seat i is assigned to Alice and seat j is assigned to Bob, the two players’ phase-shift angles are and . The probability of winning can be written as follows:

The players choose for to maximize the probability of winning. Define

and . Maximizing the probability of winning is to maximize the following expression, for ,

.

The following must be true:

Same logic applies to and . can take either +1 or -1 to maximize each term in . Then the objective function can be further restated as:

Without loss of generality, we can order so that . Then,

The maximum range so that The probability of winning is computed as . One set of strategies that could achieve this probability of winning is: . Q.E.D.

Proof of Proposition 2.

First, applying the definitions in Section 3.1, we are able to represent the quantum operation on the initial state .

Next, for a given seat assignment and the two players’ phase-shift angles, for Alice and for Bob, the probability of obtaining the state EE is computed as:

Similarly,

The probabilities of getting the same signals and getting different signals are computed, respectively, as follows:

Third, for a seat assignment ij where seat i is assigned to Alice and seat j is assigned to Bob, the two players’ phase-shift angles are and . The probability of winning can be written as follows:

Maximizing the winning probability is to maximize . Applying the identity , f(·) is rewritten as

Consider the first term in f(·), the following observation must be true: (A1)

For the second term in f(·), the following observation must be true:

(A2)

For the third term in f(·), the following observation must be true:

(A3)

Based on (A1), (A2) and (A3), f(·) is rewritten as

Let , , and so that

It is not possible to have so that f(·) can never achieve the upper bound . Note that . Due to the symmetry of f(·), we can assume so that .

Differentiating f(·) yields

The solution is or . For , and yielding . For , and yielding . The optimal winning probability is .

By setting , the values produce and . Based on , we can determine that satisfy (A1), (A2) and (A3). One possible strategy that achieving the optimal winning probability is , , ; , , and . Q.E.D

Proof of Proposition 3.

In a matrix form, the initial state is written as , which can be further written as a tensor product of two vectors, . In the initial state, the two qubits are not entangled.

Applying the definitions in Section 3.1, we are able to represent the quantum operation on the initial state .

Next, for a given seat assignment and the two players’ phase-shift angles, for Alice and for Bob, the probability of obtaining the state EE is computed as (the scale factor is 32):

Similarly,

The probabilities of getting the same signals and getting different signals are computed, respectively, as follows:

For any seat assignment, regardless of and , it is always held that . Q.E.D

## Footnotes

- footnote 1: Definition 2(iii) is a generic form of the phase shift operator that is consistent with those defined in Fellingham et al. (2026). For example, the Z-gate corresponds to , the T-gate to , and the S-gate to .
- footnote 2: In matrix form, the state is written as , which is one of the four Bell states. This state is entangled because there does not exist two vectors, and so that . Bell states are the simplest examples of quantum entanglement between two qubits.
