# Extracted text: Chapter.original.docx

Source path: /Users/ra1/QuantumAccounting/BookChapter/sources/Chapter.original.docx

## Document Body

Information Processing Using Double-Entry System in the Quantum Era

Rick Antle Yale University

John Fellingham Ohio State University

Haijin Lin University of Houston

Douglas Schroeder Ohio State University

Organizations have been profoundly reshaped by digital transformation. Core functions—from accounting and supply chain management to customer service—now rely on software, data infrastructures, and automation processes. Because organizations increasingly depend on computer-based systems to coordinate activities, changes in computational logic may influence how information is represented and managed.

The double-entry system has long served as a foundational information architecture for recording and processing economic information. Modern digital systems have largely embedded it within a classical computing framework characterized by deterministic states, sequential procedures, and binary distinctions. As quantum computing progresses from theoretical curiosity to engineering reality (Stackpole 2025), it raises a fundamental question: if computational processes increasingly rely on quantum concepts such as superposition, entanglement, and probabilistic outcomes, must the information architecture within organizations also change? More specifically, can the double-entry system continue to be relevant in the quantum era?

Our answer is yes. In this chapter, we argue that the structure and logic of the double-entry system can be used to represent fundamental quantum operations (Fellingham et al., 2025). Viewing accounting through this lens reveals structural parallels between the double-entry system and quantum information processing. These parallels suggest that the double-entry system remains relevant because its underlying information architecture extends naturally beyond the classical setting.

Our objective is not to claim that the double-entry system physically performs quantum computation, but rather that it provides a useful framework for representing and understanding key features of both classical and quantum information processing. From this perspective, the advantage of quantum computing over classical computing helps highlight the information architecture that gives double-entry system advantages over single-entry system. This lens may also provide new insights into how organizations could be designed to better exploit the information-processing capabilities shared by both the double-entry system and quantum computing.

We begin in Section 1 by examining accounting from an information science perspective. Using the three-way framing equivalence among economics, accounting, and information developed by Fellingham et al. (2022), we show that decision-making, accounting numbers, and entropy can be viewed as alternative representations of the same underlying economic activities. This equivalence establishes the double-entry system as an information-processing architecture for organizations.

In Section 2, we demonstrate that the double-entry framework can represent both classical and quantum computation. Building on the framework developed by Fellingham et al. (2025), we show how qubits, quantum gates, superposition, and conditional operations can be encoded using T-accounts and journal entries. Using these encodings, the double-entry system can represent both the Hadamard gate and the Toffoli gate, which together form a universal gate set for quantum computation. As a result, it possesses the representational capacity necessary to simulate both classical and quantum computation.

In Section 3, we extend the analysis to entanglement, one of the defining resources of quantum information processing. We first show how the entangled qubits can be constructed within the double-entry framework. We then examine the informational value of entanglement in three settings: information transmission, coordination with limited information and restricted communication, and incentives in an agency setting. Concluding remarks are offered in Section 4.

1. Double-entry System as an Information-Processing Architecture

We examine accounting from an information science perspective. Specifically, accounting is not merely recordkeeping, but a system for producing, structuring, transmitting, and using information—much like the way information science studies data, signals, codes, and communication.

Drawing on Shannon’s information theory (Shannon, 1948), which studies how uncertainty is represented, transmitted, and reduced, we treat accounting as central to managing uncertainty in organizational decision-making. In economics, organizational decisions regarding resource allocation, budgeting, and incentive contracting all rely on expectations about uncertain future states. Accounting provides the structural language—the double-entry system—through which organizational states are represented, coordinated, updated, and communicated. In this sense, the double-entry system is fundamentally an information-processing architecture.

One illustration of the information science perspective is the three-way framing equivalence developed by Fellingham et al. (2022), which shows that a firm’s economic return, accounting numbers, and the amount of information available to the firm are mathematically identical representations of the same underlying economic activities. Under this framework, a question posed in one frame can be reformulated in the other two. For example, a decision problem can be recast as an accounting problem or as an information problem. In this sense, accounting can be understood as an information science concerned with representing and processing economic states generated by organizational activities.

To establish this equivalence, we use the Kelly gambling problem—a classic problem in decision theory that yields clean and intuitive results. The analysis relies on several standard assumptions: the long-horizon decision frame, the Law of Large Numbers, and arbitrage-free pricing.

Specifically, a Kelly investor repeatedly allocates wealth across states to maximize long-run growth. Let be the probability of state i, the fraction invested, and the payoff in state i. The optimal strategy is the Kelly criterion: the Kelly investor bets a fraction of wealth equal to the probability of each state, (Kelly 1956).

In the decision frame, arbitrage-free pricing provides a consistent valuation of uncertain outcomes. The long-horizon decision frame captures the going-concern perspective, so that the decisions are made to maximize long-run growth. The Law of Large Numbers connects repeated outcomes to long-run growth. As a result, maximizing long-run average growth is equivalent to maximizing the expected log return per period. The expected log return under , denoted as E(r) in (1), is decomposed into a negative entropy term and a payoff term.

(1)

The entropy measures uncertainty about the state. When an information source M is available, the entropy and the expected log return are computed conditional on the information signals M provides. The increase in expected log-return due to M equals to the reduction of uncertainty.

(2)

This establishes the equivalence between the decision frame and the information frame.

In the accounting frame, geometric mean valuation (Hakansson, 1971) is the accounting method under which the expected log return is maximized. Under this method, the beginning book value is the initial wealth, . The end-of-period book value is written as in (3).

(3)

Income is the change in book value, , establishing the equivalence between the decision frame and the accounting frame.

(4)

Combining (2) and (4) establishes the three-framing equivalence: decision, information, and accounting.

(5)

As Fellingham et al. (2022) demonstrate, the equivalence in (5) extends to settings with quantum probabilities. Under classical probabilities, the conditional probabilities in correspond to Bayesian updating of beliefs. With quantum probabilities, the conditional probabilities reflect state revisions induced by measurement outcomes and described by quantum information theory.

This equivalence result implies that making decisions and acquiring information are equivalent activities. The quality of decisions fundamentally depends on the amount of information available. In the accounting frame, income and book value form a dual structure. Under the double-entry system, journal entries do not merely duplicate entries; they simultaneously record changes in net assets and the economic sources of these changes. Information is transmitted through the structured relations between accounts. The double-entry system functions as an information-processing architecture that encodes, updates, and communicates economic activities.

The equivalence between the accounting frame and the information frame further suggests that accounting numbers are directly linked to the probabilistic structure of the underlying economic environment. Importantly, this connection persists even when the probabilistic structure changes. The double-entry system can process information that obeys classical probability rules such as Bayes’ rule (Fellingham, 2017). Information governed by quantum probability rules may also be processed within the same system. The question then becomes how quantum information can be represented and processed within the double-entry framework. We address this question in the next section.

2. Double-Entry Representation of Classical and Quantum Computing

As developed in Fellingham et al. (2025), the four fundamental postulates of quantum information theory (Nielsen and Chuang, 2000) can be represented using T-accounts and journal entries. In this section, we use these accounting representations to illustrate the core concepts and operations of quantum information theory.

2.1 Quantum states encoded in T-accounts

The fundamental unit of quantum computing is the quantum bit (or qubit). A qubit has two basis states, state zero and state one. In the double-entry framework, these two basis states are represented by two types of accounts: account E representing state zero and account A representing state one. Both E and A have a debit balance of 1 (with 1 on the debit side and 0 on the credit side).

2.2 Quantum gates encoded in journal entries

Quantum gates are operations that transform qubit states. These operations are unitary transformations, meaning they preserve the norm of the state vector and are reversible, so that no information is lost during the transformation. Conceptually, performing a quantum gate on a qubit can be thought of as performing the operation on each basis state separately and then combining the resulting states weighted by their amplitudes. There are three types of fundamental single-qubit quantum operations: bit flip, phase flip, and phase shift.

In the double-entry framework, quantum gates are represented by journal entries. A bit-flip gate (or X-gate) swaps the two basis states and is represented by a reclassification entry that moves the balance between E and A.

(X-gate)

A phase-flip gate (or Z-gate) adds a minus sign to state one while leaving state zero unchanged. In accounting notation, it is represented by a revaluation entry that changes A between a debit balance and a credit balance while leaving E unchanged. Denote the account A with a credit balance of 1 by .

(Z-gate)

The phase-flip gate is a special case of the phase-shift gate. Whereas the phase-flip gate rotates a qubit by , a phase-shift gate (or -gate) rotates a qubit by . In accounting notation, a phase-shift gate is represented by a partial revaluation entry that either credits A or debits by an amount equal to . For example, the T-gate rotates a qubit by and is thus represented by a revaluation entry of amount , while the S-gate rotates a qubit by and thus is represented by a revaluation entry of amount 1. These revaluation entries trace out a circular structure that mirrors the unit circle in the complex plane.

More generally, quantum computation is fundamentally a process of vector transformation. The accounting notation preserves this feature by representing the basis vectors with T-accounts and vector transformation with journal entries. In this sense, the double-entry system functions as an architecture for vector processing.

2.3 Superposition encoded by the Hadamard gate

A distinctive feature of quantum information is that a qubit can exist in superposition—a linear combination of the two basis states, E and A, whose coefficients are probability amplitudes. The Hadamard gate, when applied to a basis state, creates a superposition. To understand the concept of superposition, we begin with the Hadamard gate.

The Hadamard gate (or H-gate) is a single-qubit operation that conceptually could be viewed as combining the two single-qubit operations discussed in Section 2.2: the X-gate and the Z-gate. In accounting notation, when the H-gate acts on E, the reclassification entry (X-gate) transforms E into A and the revaluation entry (Z-gate) leaves E in E. The resulting superposition state is the linear sum of these two transformations and is represented by stacking the two accounts, E and A, on top of each other, written as .

(Hadamard Gate)

Similarly, when the H-gate acts on account A, the reclassification entry transforms A into E and the revaluation entry transforms A into ; the resulting superposition state is .

The accounting notation provides an intuitive interpretation of superposition. Applying the H-gate to a basis account produces stacked rows that preserve the effects of both the reclassification and revaluation entries. Rather than reflecting one or the other, the end-of-period account is in superposition. Because accounts serve as the building blocks of financial statements, the stacked rows can be viewed as two end-of-period financial statements. Information is therefore no longer carried by a single account or a single financial statement, but jointly by multiple financial statements. In this sense, superposition allows information to be carried by two financial statements simultaneously.

2.4 Conditional operations

We now extend the discussion to multi-qubit systems and conditional operations. A composite system consists of multiple qubits combined through the tensor product. In the double-entry framework, a composite system is represented by a concatenation of accounts. For example, EA denotes a two-account system in which the first account is in state E and the second is in state A. Similarly, AEA denotes a three-account system in which the first and the third accounts are in state A and the second account is in state E.

An example of a conditional operation is the Controlled-Not (CNOT) gate, which acts on two qubits. The CNOT gate flips the state of the target qubit when the control qubit is in state A. In accounting notation, the CNOT gate is represented by a conditional reclassification entry. For example, the CNOT gate that uses the first account as the control and the second account as the target is denoted by where the first subscript denotes the control account and the second subscript denotes the target account. It transforms the system AEA into AAA because the first account is A and the second account is therefore reclassified from E to A.

(CNOT Gate)

2.5 Universality of the double-entry representation

So far, we have developed a double-entry framework capable of representing both quantum states and fundamental quantum operations. Within this framework, accounts and journal entries can be used to represent the Toffoli gate (Fellingham et al., 2025). The Toffoli gate is a three-qubit gate with two control qubits and one target qubit, and it flips the target qubit if and only if both control qubits are in state A.

The Toffoli gate is universal for classical reversible computation because it can simulate the NAND and FANOUT gates, which together are sufficient to implement any classical Boolean function. Moreover, Shi (2003) and Aharonov (2003) showed that any quantum algorithm can be approximated to arbitrary accuracy using circuits composed of only the Toffoli and Hadamard gates. Since the double-entry system can encode both the Toffoli gate and the Hadamard gate, it follows that the double-entry system is universal for both classical and quantum computation.

This result suggests that the double-entry system, as a business language for over five centuries, has sufficient structural capacity to represent quantum information processing. We conjecture that this capacity arises from the inherent symmetry and balance of debits and credits, and the reversibility of journal entries. These features preserve information through the recording process, paralleling the conservation of information in quantum information processing.

The superiority of quantum computers over classical computers arises largely from entanglement. In the next section, we explore entanglement within the double-entry framework and examine its role in information processing within organizations.

3. Entanglement and Information Processing in the Double-entry System

In quantum information theory, entanglement is treated not merely as a mysterious feature of quantum mechanics, but as a physical resource for quantum information processing (Terhal et al., 2025). We first provide an accounting representation of entanglement. Our focus is on the maximally entangled two-qubit states known as Bell states. We then demonstrate how entanglement (Bell states) functions as superior information-processing mechanism in several economic settings.

3.1. Representing entanglement in the double-entry framework

A Bell state can be generated from a two-qubit basis state in two steps. A two-qubit composite system has four basis states, written in accounting notation as EE, EA, AE, or AA. First, apply a Hadamard gate () developed in Section 2.3 to the first qubit, creating a superposition state. Second, apply a CNOT gate () developed in Section 2.4, using the first qubit as the control qubit and the second qubit as the target qubit. This operation transforms the superposition state into an entangled state. For example, beginning with the basis state EE, the two-step procedure produces , which is one of the four Bell states.

(Bell State)

The remaining three Bell states are generated analogously by applying the same two-step procedure to the other basis states. A Bell state represents two accounts maximally entangled, meaning that neither account can be fully described on its own. Together, the two accounts form a perfectly correlated structure. This is precisely the nonlocal nature of entanglement.

In accounting notation, represents an entangled state in which each account (each column) is in superposition. More importantly, the superposition state of the second account arises from its relationship with the first account, which is itself in superposition. Consequently, the informational states of the two accounts cannot be described independently of one another. The two accounts are entangled so that the information contained in the joint financial statements cannot be separately attributed to either account individually.

Accounts can become entangled through a sequence of journal entries, in particular, the H-gate followed by the CNOT gate. Neither operation by itself can generate entanglement. In organizational settings, the two accounts may represent activities, departments, or units that are geographically or functionally separated. Bell states provide a convenient way to represent such nonlocal, nonseparable relationships. In a Bell state, the two accounts are not merely uncertain individually; rather, uncertainty is shared and linked across them.

We next examine how entanglement serves as superior information-processing mechanisms in three different settings: information transmission, coordination, and incentive contracting.

3.2. Entanglement and channel capacity

We first examine whether entanglement improves the information transmission capability of the double-entry system. This question parallels superdense coding in quantum information theory, where entanglement allows a sender to transmit more classical information than would otherwise be possible through operations on a single qubit. We show that a similar informational advantage arises in the double-entry system.

An accounting system can be viewed as a communication channel. The manager (the sender) undertakes economic transactions based on private information and encodes those transactions as journal entries. The journal entries are the information-bearing messages transmitted through the accounting system. The end-of-period accounts are signals that the receiver decodes to obtain information.

A central question is how much information can be transmitted through the double-entry system. Capacity is measured in bits: one-bit capacity means the channel can reliably distinguish between two possible messages, and two-bit capacity means it can distinguish among four possible messages. More specifically, we consider four possible messages represented by the following journal entries transmitted through the channel.

I: no economic transaction occurs, so the ending state is identical to the initial state.

X: the account is reclassified.

Z: only the A account is being revalued.

(X, Z): the account is first reclassified and then revalued.

We then consider five cases in which the organizational design specification varies.

Case 1: one account in the basis state E.

Case 2: one account in superposition .

Case 3: two accounts in the basis state EE.

Case 4: two accounts that are not linked, with the first account in superposition .

Case 5: two entangled accounts in the Bell state .

As shown in Antle et al. (2026a), whether all four messages can be reliably distinguished depends on whether the organizational design specification is entangled. One-bit capacity is achieved in the first four cases. Two-bit capacity is achieved only in Case 5, where the design specification is a Bell state. To illustrate the mechanism, consider Case 5: applying the four journal entries to only the first account (the first column) produces the following results. (The subscript 1 indicates that the operation is performed on the first account.)

(Case 5 – I)

(Case 5 – X)

(Case 5 – Z)

(Case 5 – (X,Z))

The four journal entries produce four distinct end-of-period accounts, so the channel achieves two-bit capacity. Because the receiver can uniquely identify which journal entry was transmitted, two bits of information can be communicated through operations on only the first account.

Normally, one account alone carries only one bit of information as Cases 1-4 demonstrate. In Case 5, however, only one account is operated on, yet two bits are transmitted. The additional transmission capacity arises because the two accounts are entangled: the informational structure of one account is linked to the informational structure of the other.

The channel capacity result generalizes naturally to more than two accounts. That is, n-bit channel capacity can be achieved with n entangled accounts. The information transmission capacity of the double-entry system scales linearly with the number of entangled accounts.

3.3. Entanglement and strategic coordination

The channel-capacity result does not rely on any specific economic setting; it is a general result about information transmission. Economic decisions, however, are often shaped by incentives, strategic interaction, and communication constraints. We therefore next consider a game-theoretic setting—the odd-cycle game—in which entanglement may improve coordination among agents with incomplete information and restricted communication.

In the 3-seat odd-cycle game, a referee randomly assigns two players, Alice and Bob, to three seats around a round table. The seats are labeled {0, 1, 2}. There are six possible equally likely seat assignments: {00, 01, 11, 12, 22, 20}, where the first number denotes Alice’s seat and the second Bob’s seat. Each player knows only his or her own seat assignment. After the seats are assigned, the referee independently asks each player to submit a report, Red or Blue. The players win if they submit the same report when assigned the same seat and different reports when assigned adjacent seats.

Communication is restricted because the number of possible reports is strictly smaller than the number of seats. Otherwise, the players could encode their seat assignments directly and win with certainty. One pure strategy is to report Red when assigned an even-numbered seat and Blue when assigned an odd-numbered seat. This strategy wins on five of the six equally likely seat assignments and loses on exactly one, yielding a winning probability of 5/6. Moreover, no pure strategy or randomized strategy can achieve a higher winning probability.

We now consider the quantum version of the odd-cycle game. Each player is represented as an account, and the game becomes a two-account composite system. Initially, the informational relationship between the two accounts is specified. After observing his or her seat assignment, each player independently chooses a phase-shift angle ( for Bob). In accounting notation, this choice corresponds to the magnitude of a partial revaluation entry introduced in Section 2.2. These choices are implemented through a sequence of journal entries () where the subscript 1 denotes Alice’s operations and the subscript 2 denotes Bob’s. Finally, the referee measures the end-of-period accounts and computes the probabilities of the possible measurement outcomes, from which the winning probability is determined.

The analysis below compares three informational relationships between the two accounts and examines how the presence or absence of entanglement affects strategic coordination.

Case 1: The two accounts are in basis state EE. The two players act independently, and the resulting optimization problem is equivalent to the classical odd-cycle game. The maximum winning probability attainable remains 5/6. Thus, quantum strategies offer no advantage in this case.

Case 2: The two accounts are in the Bell state , so the two accounts are entangled. The maximum winning probability increases to 1/2 + √3/4 ≈ 0.933, strictly exceeding the classical ceiling of 5/6 ≈ 0.833. Entanglement links the two accounts and allows them to coordinate more effectively than is possible in the classical game.

Case 3: The two accounts are represented by , so the first account is in superposition while the two accounts remain independent. The maximum winning probability falls to 1/2, which is strictly below the classical benchmark of 5/6. In this case, superposition alone does not improve coordination.

The comparison of the three cases suggests several insights. First, entanglement is the source of the coordination advantage. By structurally linking the two accounts, entanglement creates dependence between their outcomes and enables coordination through a shared informational structure in a way that is impossible when the accounts operate independently. As a result, the accounts achieve a level of coordination that exceeds the classical benchmark.

Second, our analysis reveals the distinct roles of the H-gate and the CNOT gate in generating entanglement. Case 1 includes neither gate and reproduces the classical benchmark. Case 3 includes the H-gate but not the CNOT gate, placing one account in superposition without linking it to the other account. Superposition without entanglement is not merely insufficient—it can be detrimental. Only in Case 2 are both the H-gate and the CNOT gate present. The coordination advantage therefore arises from entanglement.

Third, the comparison highlights an important distinction between single-entry and double-entry systems. The classical odd-cycle game is analogous to a single-entry system because accounts submit reports directly and no journal-entry structure underlies the decision process. By contrast, the quantum version is analogous to a double-entry system because the underlying operations are implemented through journal entries. The value of the double-entry system lies not merely in recording information twice, but in linking information across accounts. Our analysis suggests that the double-entry system can always simulate the single-entry system (Case 1). More importantly, the links created by the double-entry system can entangle accounts (Case 2), enabling coordination outcomes that independent single-entry records cannot replicate.

3.4. Entanglement and performance measurement

The odd-cycle game illustrates how entanglement improves information processing in a setting where communication is restricted. In that setting, entanglement creates an informational linkage between players, enabling nonlocal coordination that cannot be achieved classically. Organizations use information not only to communicate and coordinate but also to produce. Productive activities often depend on interactions among individuals, and the contribution of one individual may depend fundamentally on the actions of others. When production depends on such interactions, the informational linkages may also influence organizational performance and the design of performance measurement systems. In this way, entanglement becomes a productive resource.

Consider a principal-agent setting involving two agents whose productivity depends on their ability to work together. The principal seeks to induce effort through incentive contracts and can choose between two measurement systems. Under individual measurement, each agent's performance is evaluated and observed independently. Under group measurement, only the joint performance outcome is observed. This is the setting developed in Demski et al. (2008). Three cases are examined that differ in the extent to which the productive output depends on interactions between the agents—that is, the degree of synergy.

Case 1: no synergy. The two agents work independently, so productive output is simply the sum of their separate contributions. In this case, individual performance measures provide useful information and generally outperform group measurement. This is the standard result in agency theory: more detailed information improves incentive contracting when productive activities are separable.

Case 2: pure synergy. The two agents are fully interdependent, so productive output arises entirely from their interaction. In this case, attempting to measure each agent separately destroys the informational linkage underlying joint production. Group measurement, although less informative about individual effort, preserves that structure and therefore dominates individual measurement.

Case 3: partial synergy. The agents are neither fully independent nor fully interdependent. In this intermediate case, the preferred measurement system depends on the degree of synergy. Below a threshold, individual measurement dominates. Above the threshold, group measurement dominates. Most importantly, as the agency problem becomes more severe, the threshold decreases and the range over which group measurement dominates expands.

In the agency setting, entanglement contributes directly to production. When the two agents work interdependently, productive output arises entirely from their interaction. Group measurement, although less informative about individual efforts, preserves the linkage structure between the agents’ productive activities and therefore dominates individual measurement. While synergy describes the productive value generated by interaction among agents, entanglement is the informational structure that supports that interaction. In this sense, entanglement functions as a productive resource, encouraging the use of synergy in the production.

One interesting finding is that as the agency problem becomes more severe, the range over which group measurement dominates expands. This result is counter-intuitive because conventional wisdom suggests that more severe agency problems require more measurement and tighter monitoring. Yet the analysis shows that precisely when the incentive to monitor increases, individual measurement can become more harmful. Additional measures may reduce efficiency if they encourage agents to focus on separate signals rather than on joint performance. The lesson is that when coordination matters, preserving entanglement among agents becomes increasingly valuable.

Finally, the results connect directly to the underlying accounting systems. Individual measurement is analogous to treating accounts as separate records, while group measurement is analogous to preserving the links among accounts within a double-entry system. The value of the double-entry system lies in preserving and processing the relationships among organizational activities. In this way, entanglement again appears as the valuable organizational resource.

4. Concluding Remarks

This chapter has examined the double-entry system from an information science perspective and argued that it remains relevant in the quantum era. Building on the three-way framing equivalence among decision-making, information, and accounting, we first showed that the double-entry system functions as an information-processing architecture through which economic information can be represented, updated, and communicated. We then demonstrated that the fundamental elements of quantum information processing—including qubits, quantum gates, superposition, and conditional operations—can be represented within the double-entry framework. Because the framework can represent both the Hadamard gate and the Toffoli gate, the double-entry system possesses the representational capacity necessary for both classical and quantum computation.

The central insight is that the informational advantage of the double-entry system arises from entanglement. When the structural linkages among accounts are preserved, the double-entry system processes information in the way that cannot be achieved classically. Moreover, we show that entanglement is valuable (i) by expanding the communication channel capacity by allowing two bits to be communicated through one single account, (ii) by creating the linkage among players for better information processing in a coordination game with restricted communication, and (iii) by encouraging agents to pay more attention to synergy and joint performance rather than individual performances. These settings—information transmission, coordination, and incentives—highlight the major organizational decisions, and in each, the advantages appears only when the nonlocal informational linkages among accounts (entanglement) are preserved and disappears when those linkages are broken.

Our analyses offer an explanation for the remarkable durability of the double-entry system. Information theory suggests why the double-entry system has survived more than five centuries of economic and technological change with little modification to its fundamental structure. The double-entry system supports vector processing, enables superposition, and preserves informational relationships that would otherwise be lost. These features increase the system’s capacity to organize, communicate, and process economic information. A single-entry system, in contrast, functions as a scalar processor and lacks this relational structure. It thus cannot achieve the same informational performance. Whenever valuable information resides in the relationships among accounts rather than in individual accounts, a structure that preserves these relationships—and therefore preserves entanglement—can outperform one that separates them.

Our analyses also possess pedagogical value. Each of the four postulates of quantum information theory receives a natural accounting interpretation: qubit states encoded as T-accounts, unitary evolution encoded as journal entries, composite systems as concatenations of accounts, and measurement as the determination of ending balances with probabilities governed by amplitudes (Fellingham et al. 2025, Fellingham et al. 2026). For researchers, educators, and practitioners in business, this framework makes quantum information theory accessible. As quantum computing transitions from theoretical possibility to engineering reality, the double-entry system serves as an information-processing architecture whose structural logic is compatible with core principles of quantum information processing.

References

Aharonov, Dorit. 2003. “A simple proof that Toffoli and Hadamard are quantum universal.” arXiv:quant-ph/0301040.

Antle, Rick, John Fellingham, Haijin Lin, and Doug Schroeder. 2026a. “The channel capacity of the double-entry system.” Working paper.

Antle, Rick, John Fellingham, Haijin Lin, and Doug Schroeder. 2026b. “Double-entry accounting, entanglement, and odd-cycle game.” Working paper.

Demski, Joel, John Fellingham, Haijin Lin, and Doug Schroeder. 2008. “Interaction between productivity and measurement.” Journal of Management Accounting Research 20: 169-190.

Fellingham, John. 2017. Accounting: An Information Science. Available at https://bpb-us-w2.wpmucdn.com/u.osu.edu/dist/5/39171/files/2016/10/Fellinghambook-with-rev-8-2bof2wx.pdf.

Fellingham, John, Haijin Lin, and Doug Schroeder. 2022. “Entropy, double entry accounting and quantum entanglement.” Foundations and Trends in Accounting 16 (4): 308-396.

Fellingham, John, Haijin Lin, Doug Schroeder. 2025. “Using double-entry accounting to program quantum computers.” Working paper.

Hakansson, Nils H. 1971. “Multi-period mean-variance analysis: toward a general theory of portfolio choice.” The Journal of Finance 26 (4): 857-884.

Kelly, John L. 1956. “A new interpretation of information rate.” The Bell System Technical Journal 35 (4): 917-926.

Nielsen, Michael A., and Isaac L. Chuang. 2000. Quantum Computation and Quantum Information. Cambridge University Press.

Odrzywolek, Andrzej. 2026. “All elementary functions from a single binary operator.” arXiv:2603.21852.

Shannon, C. E. 1948. “A mathematical theory of communication.” The Bell System Technical Journal 27 (3): 379-423.

Shi, Yaoyun. 2003. “Both Toffoli and Controlled-Not need little help to do universal quantum computing.” Qunatum Information & Computation 3(1): 84-92.

Stackpole, Beth. 2025. “Quantum Computing Reality Check: What Business Needs to Know Now.” Ideas Made to Matter, MIT Sloan School of Management. https://mitsloan.mit.edu/ideas-made-to-matter/quantum-computing-reality-check-what-business-needs-to-know-now.

Terhal, Barbara M., Michael M. Wolf, and Andrew C. Doherty. 2025. “Quantum entanglement: a modern perspective.” Physics Today (January): 40-46.

## Footnotes

- footnote 1: In this sense, the Kelly investor can be viewed as a decision maker with log utility.
- footnote 2: For detailed derivations, please refer to Fellingham et al. (2022).
- footnote 3: Fellingham (2017, chapter 7) demonstrates that the T-account structure mirrors the stock-and-flow mechanics of Bayesian revision. A decision maker begins a period with prior beliefs (stocks) about uncertain future cash flows, observes evidence during the period (flows), and updates to posterior beliefs (revised stocks). Under an appropriately chosen amortization rate, standard journal entries recursively transform prior states into posterior estimates while preserving the same structural relation between beginning and ending balances. In this sense, the stock account functions as a mechanism that perpetually performs Bayesian updating, period after period.
- footnote 4: The reclassification entries are Debit A / Credit E by 1 and Debit E / Credit A by 1.
- footnote 5: The revaluation entries are Debit Gains/Losses / Credit A by 2 and Debit A / Credit Gains/Losses by 2.
- footnote 6: The -gate will be used in the quantum odd-cycle game presented in Section 3.3.
- footnote 7: The entry for the T-gate, Debit Gains/Losses / Credit A by ½, changes A from a debit balance of 1 to a debit balance of ½, and the entry, Debit A / Credit Gains/Losses by ½, changes from a credit balance of 1 to a credit balance of ½. Similarly, the S-gate changes both A and to a zero balance. In T-account notation, the entry for the S-gate, Debit Gains/Losses / Credit A by 1, changes A to an account with 1 on both the debit and credit sides, and the entry, Debit A / Credit Gains/Losses by 1, changes to an account with 2 on both the debit and credit sides. These accounts form a circle analogous to the unit circle in the complex plane. A more detailed discussion can be found in Fellingham et al. (2025).
- footnote 8: The Hadamard gate is written as , where the amplitude is important to ensure that the H-gate is unitary. In our accounting notation, this factor is recorded separately for expositional clarity.
- footnote 9: In Fellingham et al. (2025), the Toffoli gate is decomposed into a sequence of sixteen operations (sixteen journal entries composed of X-, H-, S-, and T-gates). This step-by-step accounting notation makes it transparent how the Toffoli gate acts on a three-qubit state, including the creation and removal of superposition and the application of CNOT operation on the target qubit.
- footnote 10: Universality refers to the principle that a small collection of primitive operations can generate a rich class of structures. Recent work by Odrzywolek (2026) demonstrates this idea by showing that a single binary operator can generate the broad class of elementary mathematical functions. Because the double-entry framework admits representations of the Hadamard gate and the Toffoli gate, it is universal for representing classical and quantum computations.
- footnote 11: Non-locality is a defining feature of Bell states (entanglement). In classical systems, correlations between two separate accounts can be traced to locally stored information: each account carries its share of a common signal. Entangled accounts, however, exhibit correlations that cannot be decomposed in this way. In a Bell state, neither account has a definite informational state on its own. Instead, the information is embedded in the relationship between the accounts. In this sense, entanglement is nonlocal. In organizational terms, when accounts are entangled, examining a single account cannot recover the full information content of the system. That content only exists at the level of the relationship—a structure that the double-entry framework is uniquely suited to represent and preserve.
- footnote 12: Please refer to Antle et al. (2026a) for more detailed analysis.
- footnote 13: Please refer to Antle et al. (2026b) for more detailed analysis.
- footnote 14: Using the accounting notation developed in Section 2, the no-synergy case is described by EE, and the pure-synergy case is described by . The individual measurement system uses the basis states, EE, EA, AE, and AA, as the measurement basis. The group measurement system uses the Bell states, , , , and , as the measurement basis. The end-of-period accounts are obtained after applying the journal entries . The principal then computes the probabilities of possible performance outcomes and determines the probability of success. Thus, the setting in Demski et al. (2008) can be represented within the same framework used to analyze the odd-cycle game (Section 3.3), with the key difference being that the agency setting introduces conflicts of interest and incentive contracting.
