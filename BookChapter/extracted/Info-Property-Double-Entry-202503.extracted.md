# Extracted text: Info-Property-Double-Entry-202503.docx

Source path: /Users/ra1/QuantumAccounting/BookChapter/sources/Info-Property-Double-Entry-202503.docx

## Document Body

An Information Property of Double Entry Accounting

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

March 2025

Abstract

This paper studies the information effect of double entry accounting. In particular, we explore the information transmission capacity of the double entry accounting. To do so, the double entry accounting is depicted as a communication channel with T-accounts and journal entries where T-accounts are a two-element vectors and the (non-cash) journal entries are two-by-two matrices. All (non-cash) transactions boil down to four basic journal entries. An accounting system achieves two-bit information transmission capacity as long as one account can communicate four entries and produce four distinct signals. This requires that information should be recorded on more than one statement (the entanglement property) and information recorded should satisfy the accounting identity and the cash flow reconciliation identify (the articulation property). Our study demonstrates that the double entry accounting is an efficient information communication channel.

I. Introduction

Double-entry system is an accounting system with several salient features. In this paper, we revisit these features and explore an information property of the double-entry system. The focus is on the structure of the double-entry system, not the accounting data—the product of the double-entry system. There is a vast literature studying the properties of accounting data and its use. Accounting data is viewed as information that facilitates decision-making, control and evaluation. It is well understood that the value of accounting data cannot be determined independent of how the accounting data is used (Demski 1973). However, the literature on understanding information properties of the structure that produces accounting data is lacking.

The aim of this paper is to explore the information transmission capacity of the double-entry system. Intuitively, an accounting system can be viewed as a communication channel a sender uses to transmit messages; the accounting data is the signal that a receiver uses to infer the sender’s messages. Even though the desirable information signals vary in different context, the underlying accounting structures that produce these signals are quite similar. This observation allows us to examine the information property of the accounting structure without specifying how the signals are used.

We adopt the information theory pioneered by Hartley (1928) and Shannon (1948) to model an accounting system as a communication channel. The journal entries are the (encoded) messages represented by two-by-two matrices; the T-accounts are the signals represented by two-element vectors; and the communication is to post journal entries to T-accounts (essentially multiplying vectors and matrices). Effects of scale are removed from the analysis. This is done in order to focus on the information effects of the double-entry structure, rather than the dollar amounts. As scale is removed, all the T-accounts effectively have a balance of one. If the balance of one is on the debit (credit) side of the T-account, the T-account will be labeled as either an asset or an expense (either a liability or a revenue). Hence, a T-account carries one bit of information. This is analogous to a (fair) coin carrying one bit of information either a head or a tail.

Information processing capability lies in the two types of non-cash entries, reclassification and revaluation. In our thought experiments, it is sufficient to consider four journal entries (or messages): a reclassification, a revaluation, a reclassification followed by a revaluation, or no journal entry, in the sense that any combinations of reclassification entries and revaluation entries can be represented by one of these four entries. The four messages comprise two bits of information. As the thought experiments show, one account can transmit two bits of information but not without the presence of a second account. The two-bit capacity obtains even though the second account remains unchanged.

The two-bit channel capacity is determined by two properties of the double-entry system, the superposition property and the articulation property. In accounting, we emphasize the cash-accrual duality. Transactions are recorded on the accrual statements, the balance sheet/the income statement, and the cash flow statement. The superposition property of the double-entry system combines the effects of the accrual statements and the cash flow statement. How information is recorded on one financial statement is not as important as how information is recorded on multiple financial statements from the channel capacity perspective. The articulation property prescribes how information should be recorded on multiple statements. In particular, encoding a transaction satisfies both the accounting identity and the cash flow reconciliation identity so that the accrual and the cash flow statements articulate. When there are at least two accounts satisfy the articulation property even though the two accounts are not related, the two-bit channel capacity is achieved

Our paper contributes to the understanding of the double-entry system by identifying the features of the double-entry system that would make it most efficient in transmitting information. Paton (1917) states that the essence of the double-entry system is to maintain equality between two fundamentally distinct classes, property and equities. Ijiri (1989) states, “What is important in a system of double-entry bookkeeping is not just that each transaction is being entered in two different accounts, but that transactions are accounted for by two systems of accounts (Ijiri 1989, p. 28).” Basu and Waymire (2021) state what makes the double-entry system differs from the single-entry system is the recognition of revenues and expenses from individual transactions; the two entries and the constraint of debits equal credits increase the demand for accounting knowledge. We agree with Ijiri (1989) and Basu and Waymire (2021) that explaining any net changes of wealth using income accounts (i.e., the income statement) is meaningful and adds information. We also observe that the reconciliation between net income and net changes in cash (i.e., the cash flow statement) is necessary to achieve maximum information communication capacity.

Our paper provides an explanation for why the double-entry system has survived an explosion in the complexity of economic organizations, transactions and information for over fifty decades with little changes. Littleton (1928) raises a similar question while discussing the characteristic theory, form and technology of the double-entry system. He explained that the modern economic development over 434 years only affected and changed the characteristic theory of transaction analysis, but not the characteristic form and technology. Our study complements Littleton (1928) and further explains that the form and the technology of the double-entry system constitute an information communication channel. This is why the double-entry system could adapt to any economic advances that require information.

Arya, Fellingham, Glover, Schroder and Strang (2000) represent the double entry process using an incidence matrix (and a directed graph) and ask how much information (transactions) a user could infer from the incidence matrix. They show that the user’s ability to infer transactions is constrained by the null-space of the incidence matrix. We complement this line of research by stressing: one, the double-entry system is modeled as a communication channel where transactions are represented by the two-by-two transformation matrices; and two, whether a receiver infers transactions (journal entries) is determined by the articulation of the financial statements.

The outline of the paper is as follows. Section II describes the basics of an accounting system and provides the vector representation for the T-accounts and the types of the journal entries. In Section III, we present thought experiments in which a sender transmits four messages in a system using one account on one financial statement, two financial statements with one account on each statement, two accounts on one financial statement, and two financial statements with two accounts on each statement. We identify that there is only one out of the four experiments where four messages (that is, two bits of information) are transmitted. Section IV provides an accounting interpretation of the findings in Section III by connecting the salient features of the double-entry structure with the findings. Section V provides some extensions to show the robustness of our findings. We conclude in Section VI. All the proofs are provided in Appendix A. The comparison between the formulation of the double-entry system with the axioms in the quantum information theory is discussed in Appendix B.

II. Basics of The Double-entry System

2.1 Accounts

We consider four accounting objects (asset (A), expense (E), liability (L), or revenue (R)). The object A represents a non-cash asset account (e.g., receivables, equipment, or investment). Cash account is used separately whenever needed. Because our primary interest is on the information property of an accounting system, we abstract away from the scale issues and all accounts will have a balance of one. In our analysis, an account with a debit balance 100 is treated the same as the account with a debit balance 1.

Assumption 1. An asset or an expense account is a T-account with a debit balance of one; a liability or a revenue account is a T-account with a credit balance of one.

Just as one bit of information is represented by 0 and 1 in information theory, we can try to use 0 and 1 to represent the four accounts, A, E, L, and R. This turns out to be too restrictive because using 0 and 1 only yields three possible values, 0, 1, and -1, to represent three accounts. A two-element vector with zeros and ones allows us to represent the four unit-accounts.

Definition 1. An account is represented by a two-element vector. Define an expense account by the vector [1 0] and an asset account by the vector [0 1]. Similarly, define a revenue account and a liability account as -1 times an expense account and an asset account, respectively. In particular,

We can adopt the notion of distinct signals in the information theory and apply it to accounting. In particular, vectors [0 1] and [1 0] are distinct because these two vectors are orthogonal (i.e., their dot product is zero). On the other hand, vectors [0 1] and [0 -1] are indistinguishable in the sense that [0 -1] is a scalar multiple of [0 1], meaning they span the same one-dimensional subspace and are perfectly correlated.

Definition 2. (i) The accounts on the balance sheet (the stock accounts) are distinct from the accounts on the income statement (the flow accounts). (ii) The accounts on the same financial statement are indistinguishable.

In accounting, capitalizing and expensing a cash expenditure represent two distinct signals (Definition 2(i)). To understand Definition 2 (ii), an asset with a credit balance is a “negative asset” and can be represented by the vector [0 -1]. Structurally, a negative asset is equivalent to a liability account. An asset and a negative asset are not distinct and indistinguishable. Similarly, a liability with a debit balance is a “negative liability,” structurally equivalent to an asset account and represented by the vector [0 1]. For convenience, a negative asset is denoted by = [0 -1] and a negative liability by = [0 1].

2.2 Journal entries—X and Z operations

There are three types of journal entries: recognition, reclassification and revaluation. A recognition entry occurs when an accounting object first enters the accounting system. The entry typically (but not always) involves Cash as one of the accounts, for example, Debit Equipment Credit Cash.

Both the reclassification entry and the revaluation entry are non-cash entries. A reclassification entry changes an accounting object from an asset to an expense or vice versa (for example, Debit Depreciation expense Credit Equipment). Likewise, liabilities can be reclassified as revenues or vice versa (for example, Debit Unearned revenue Credit Revenue). A revaluation entry changes the amounts assigned to an accounting object (in particular, asset or liability).

The non-cash entries employ any two of the four unit-accounts (A, E, L and R). In Definitions 3 and 4, we represent the reclassification entry by an X-operator and the revaluation entry by a Z-operator.

Definition 3. An X-operator represents a general reclassification entry so that an asset is reclassified as an expense or an expense is reclassified as an asset, denoted by .

Similarly, a corresponding relationship for the liabilities account and the revenues account is denoted by L.

An X-operator is reversible—that is, starting with an asset account and applying the X-operator twice yield an asset (). This property of the X-operator can be easily explained with an accounting example. Start with a receivable account. The first X-operator is to estimate a bad debt expense (Debit Bad debt expense Credit Accounts receivable). As a result, the balance of the receivable account is zero. When the payment collection is expected, it is necessary to reverse the entry and to reclassify the bad debt expense account as the receivable account (Debit Accounts receivable Credit Bad debt expense). The second X-operator restores the receivable account.

Definition 4. A Z-operator represents a general revaluation entry that an asset is revalued downward to a negative asset or a negative asset revalued upward to an asset, denoted by . Similarly, .

| Revaluing an asset | Revaluing a liability |
| --- | --- |
|  |  |
|  |  |

Revenues and expenses are not revalued so that and .

Similar to the X-operator, the Z-operator is also reversible—that is, applying the Z-operator twice would eliminate any gains or losses ().

In modeling an accounting system as a communication channel, recognition entries—such as when cash is received or paid—introduce accounts (A, L, R and E) into the system. In contrast, non-cash entries—specifically reclassification X and revaluation Z—represent the messages that the managers try to transmit through the accounting system. This raises a question: are the X and the Z operators sufficient to describe all the non-cash transactions? If any non-cash transactions can be represented by a combination of the reclassification entries (X) and the revaluation entries (Z), then we say that the X and the Z operators are considered complete, in the sense that the message space of the manager can be sufficiently defined by X, Z and combinations of X and Z. The following observation summarizes the finding.

Observation 1. The reclassification (X) and the revaluation (Z) operators are complete in the sense that a non-cash account can be reached from any other non-cash accounts with a combination of the X-operators and the Z-operators.

Figure 1 illustrates Observation 1 where any entry with two unit-accounts can be represented by a combination of the X and the Z operators. Note that all the arrows are double sided because X and Z are reversible.

Figure 1: The completeness of X and Z operators

For example, a journal entry of Debit Expense Credit Liabilities can be achieved by two entries, Debit Assets Credit Liabilities and Debit Expense Credit Assets, in short, the operator “ZX.”

As we show in the proof of Observation 1, any combination of the X- and the Z- operators boils down to one of the following four operations: I-operator (no journal entry), X-operator (reclassification), Z-operator (revaluation), or (X, Z). The last operation means X and Z are performed sequentially in the order of the X-operator the first and the Z-operator the second. For completeness, the I-operator denotes no entry. These four operations are sufficient to describe all the non-cash entries for an entity during a fiscal period and thus are not restrictive.

In our setup, the four operations define four possible messages the sender (the manager) transmits through the accounting system. If four (distinct) signals are produced, we say two-bit information is transmitted and the accounting system achieves maximum information transmission capacity.

III. Analyzing the Double Entry System as a Communication Channel

In this section we describe an accounting system as a communication channel using accounts and journal entries. The initial state is determined by a recognition entry under which cash is paid and either an asset (A) or an expense (E) is recognized. A sender transmits four messages (defined by reclassification and/or revaluation operations), I, X, Z, and (X, Z), which in turn changes the state. A receiver obtains a signal to infer the sender’s message. Four distinct signals imply two-bit channel capacity.

We run four thought experiments to determine how many bits of information one account can transmit. The sender can use one account (i.e., one vector) from one financial statement (as in Section 3.1), or two financial statements and one account from each statement (i.e., two vectors stacking together as in Section 3.2). The sender can also use one account while appending a second account but keeping it intact (as in Sections 3.3 and 3.4). There are no other structures imposed.

3.1 Communication using one account on one financial statement

The first experiment is a scenario where a sender uses one account from one financial statement to transmit messages. The one account can be either an E on the income statement or an A on the balance sheet. Suppose an expense account (E) is used to send the four messages. Applying the messages (I, X, Z, or (X, Z)) to the expense account yields four signals.

Applying I to E yields E.

Applying X to E yields A.

Applying Z to E yields E.

With (X, Z), first applying X to E yields A then applying Z to A yields .

| Table 1: Example 1—using an expense account to transmit messages | Table 1: Example 1—using an expense account to transmit messages |
| --- | --- |
|  |  |
|  |  |

There are three signals {A, E, } produced; as Example 1 in Table 1 shows, because A = [0 1] and =[0 -1] are indistinguishable by Definition 2, there are effectively two distinct signals, A and E. Hence, one bit of information is transmitted.

Using an asset account (A) to send the four messages yields four signals.

Applying I to A yields A.

Applying X to A yields E.

Applying Z to A yields .

With (X, Z), first applying X to A yields E then applying Z to E yields E.

| Table 2: Example 2—using an asset account to transmit messages | Table 2: Example 2—using an asset account to transmit messages |
| --- | --- |
|  |  |
|  |  |

There are two distinct signals, A and E, and one-bit channel capacity is obtained (as shown in Table 2).

3.2 Communication using one account from two financial statements

The recognition entry can be recorded on multiple financial statements. In the second experiment, the sender employs two financial statements and one account from each statement to transmit messages.

Definition 5. The representation of two financial statements is defined as having two rows and each row representing one financial statement.

Table 3 presents an example in which E is on both statements, denoted as . To retrieve the signal, the two vectors are added up and the sum vector is scaled to a vector with zeros and ones. Adding the two vectors yields a sum vector [2 0]; and multiplying 1/2 produces a signal [1 0].

| Table 3: Signal from two financial statements with an E in each statement |
| --- |
|  |

Using an E or an A for each statement, there are four possible scenarios, , , or . We do not impose any structures about how the accounts on two financial statements are related. The operations are applied to both statements. Suppose the sender uses to transmit messages and consider the X-operator. Applying X to A on the top statement yields an E and the E on the bottom statement yields an A; thus, the signal is (see the upper right corner of Table 4).

| Table 4: Example 3—using E on the top statement and A on the bottom statement to transmit messages | Table 4: Example 3—using E on the top statement and A on the bottom statement to transmit messages |
| --- | --- |
|  |  |
|  |  |

As Example 3 in Table 4 shows, if is used to transmit messages, two distinct signals are produced, [1 -1] and [1 1]. Thus, one bit of information is transmitted. It is straightforward to check that in all four scenarios, one-bit channel capacity is obtained.

3.3 Communication using two accounts on one financial statement

A chart of accounts, a list of all the accounts an entity has, is an important component of the accounting system. For our purpose, it is meaningful to examine the information transmission capacity of one account in the presence of another account. In the third experiment, we consider a two-account structure in which the sender uses the first of the two accounts to transmit messages.

In vector representation, two accounts can be combined using tensor product (denoted by ). Combining an expense account and an asset account yields four possible four-element vectors (as shown in Table 5).

| Table 5: Two accounts constructed with A and E | Table 5: Two accounts constructed with A and E |
| --- | --- |
|  |  |
|  |  |

Definition 6. Two accounts can be represented by a four-element vectors with zeros and ones, a tensor product of two accounts.

As Example 4 in Table 6 shows, the sender uses an expense account to transmit messages while an asset account is present (the initial state is EA). The operations are only applied to the first account but not to the second account (as indicated by the subscript 1). For example, applying to EA yields AA as the first account “E” changes to “A” and the second account “A” does not change.

| Table 6: Example 4—using the first account in EA to transmit messages | Table 6: Example 4—using the first account in EA to transmit messages |
| --- | --- |
|  |  |
|  |  |

In this scenario, three signals are produced, EA, AA, and A. Since the vectors [0 0 0 -1] is a scalar multiple of [0 0 0 1], AA, and A are not distinct. Consequently, one-bit capacity is obtained.

So far, in all the three thought experiments, one-bit information capacity is obtained. Our findings are summarized in the following proposition.

Proposition 1. Two-bit channel capacity is not achieved when the initial state is defined (i) using one account from one financial statement; or (ii) using two financial statements and one account on each statement; or (iii) using two accounts from one financial statement.

3.4 Communication using two financial statements and two accounts from each statement

The last experiment is to consider two financial statements with two accounts on each statement. This structure can be represented by two rows and a four-element vector on each row. A signal is the (scaled) sum vector by adding the two four-element vectors. One such example is presented in Table 7.

| Table 7: Vector representation of two financial statements with AA on the top statement and EE on the bottom statement |
| --- |
|  |

In this structure, the rows are the financial statements and the columns are the accounts. The operators are applied to the first column (the first account on both statements) and the second column (the second account on both statements) does not change.

| Table 8: Example 5—using the first account to transmit messages with two financial statements, AA on the top statement and EE on the bottom statement | Table 8: Example 5—using the first account to transmit messages with two financial statements, AA on the top statement and EE on the bottom statement |
| --- | --- |
|  |  |
|  |  |

As Example 5 in Table 8 shows, if the sender uses the first column in to transmit messages, the receiver obtains four signals, orthogonal to each other and hence distinct. Four distinct signals convey two bits of information and thus, two-bit channel capacity is obtained.

There are possible scenarios, depending on whether there is an E or an A for each account on each statement. The next question is whether the two-bit channel capacity is obtained in all 16 scenarios. This is not true.

| Table 9: Channel capacity with two financial statements and two accounts | Table 9: Channel capacity with two financial statements and two accounts |
| --- | --- |
| Scenarios with two-bit capacity | Scenarios with one-bit capacity |
| ; ; ; | ; ; ; ; ; ; ; ; ; ; |

In fact, among the 16 scenarios, there are 12 scenarios in which the accounting system does not have two-bit capacity (as shown in the right column of Table 9); while in the other 4 scenarios the two-bit capacity is obtained (as shown in the left column of Table 9). In each of these four scenarios, there are exactly an A and an E in each column.

Proposition 2. Two-bit channel capacity can be achieved in a scenario where there are two financial statements and two accounts on each statement if, and only if, each account (represented by a column) has exactly an A and an E.

IV. An Accounting Interpretation

In this section, we provide an accounting interpretation for Proposition 2 and in particular, we describe the salient features of the double-entry system that could explain the initial states in the four scenarios as specified in the left column of Table 9. That is, there are two financial statements and two accounts on each statement; each account (each column) has an E and an A between the two statements.

4.1 The salient features of the double-entry system

In accounting, transactions are often recorded on more than one financial statement. For example, sales or expenses are reported on the income statements, but also included in the ending balance of Retained Earnings on the balance sheet. For another example, accrual transactions are reported on the balance sheet and/or the income statement, but also reported on the cash flow statement (using indirect method). The receiver infers messages being transmitted from a signal that combines reporting from multiple financial statements. This is the superposition property of the double-entry system.

Definition 7. The superposition property of the double-entry system combines two financial statements into one vector representation. How information is recorded on one financial statement is not as important as how information is recorded on all financial statements from the channel capacity perspective.

The superposition property prescribes the two-row structure. Without loss of generality, we consider the two financial statements in our vector presentation as one accrual statement and one cash flow statement. Next, we demonstrate that the articulation of the financial statements guarantees the structure of one E and one A for each column.

Definition 8. Under the double-entry system, the following two identities always hold at any point in time so that the financial statements articulate.

The accounting identity, Assets = Equities, prescribes the accrual statement (including the balance sheet and the income statement).

The cash flow reconciliation identity, , reconciles the accrual-based income and the net changes in cash and prescribes the statement of cash flows.

Going back to our experiments in which the initial state is defined as cash paid and either an asset (A) or an expense (E) recognized. The accounting identity holds if the changes of equities equal the change of assets. In particular, Income equals the sum of the changes in cash and the changes in (non-cash) assets (denoted by ).

(1)

The cash flow reconciliation identity holds if the net changes in Cash equal to Income minus the adjustments such as cash expenditures (denoted by ).

(2)

Adding (1) and (2) yields

(3)

The equality (3) states that the changes of non-cash assets equal the adjustments made to Income on the cash flow statement so that the accrual statement and the cash flow statement articulate.

We use (3) to explain the initial state in Table 9. For ease of exposition, the top statement represents an accrual statement and the bottom statement represents a cash flow statement. On the accrual statement, an “A” represents an asset and an “E” represents an expense. On the cash flow statement, an “A” represents no adjustment needed and an “E” represents cash expenditure.

If an asset is recognized on the balance sheet (an “A” on the top statement), a cash expenditure should be recorded on the cash flow statement (an “E” at the bottom statement). This is coded as in the experiments. If an expense is recognized on the income statement (an “E” on the top statement), there is no adjustment needed on the cash flow statement (an “A” at the bottom statement). In our experiment, this is coded as .

Lemma 1 When the (cash) recognition entry is processed under the double-entry system where the financial statements are always articulate (meaning both the accounting identity and the cash flow reconciliation identity hold), the structure of one account on two financial statements must be either or .

Lemma 1 demonstrates that the articulation of the two financial statements (two rows) yields the structure of one A and one E in each column. As long as a column has an E and an A, the two financial statements must articulate. The structures with two As or two Es do not ensure the articulation of the financial statements. To see this, means that an asset is recognized on the balance sheet and there is no adjustment on the cash flow statement. In this case, the accounting identity holds.

Accounting identity

But the cash flow reconciliation identity does not hold because of an omission error.

Cash flow reconciliation identity

Similarly, means that an expense is recorded on the income statement and there is an adjustment on the cash flow statement. In this case, the accounting identity holds.

Accounting identity

But the cash flow reconciliation identity does not hold because of a double counting error.

Cash flow reconciliation identity

Recall the structure of the states (in Table 9) has two rows (representing two financial statements) and two columns (representing two accounts). The superposition property explains the two-row structure. The articulation property explains the column structure. We now restate Proposition 2 by directly linking the features of the double-entry system with its ability to achieve the maximum information communication capacity. Although the second account (i.e., the second column) does not transmit information, it is essential for achieving the two-bit channel capacity that the second column has an E and an A.

Proposition 3 One account can transmit two bits of information under the double-entry system with the superposition property when there are two accounts and both accounts satisfy the articulation property (that is, in the structure of or ).

4.2 An accounting example

So far, we demonstrate the entanglement property for cash transactions (i.e., recognition entries). Our next question is whether the entanglement property holds for the non-cash entries, the X and the Z operators. As long as the entanglement property holds (that is, one E and one A in each column), two-bit channel capacity is always achievable.

If the initial state takes the format of either or for each column, applying the X-operator switches an E to an A or an A to an E; thus, each column has exactly an A and an E. The revaluation entry imposes a scaling effect to change an A to an while does not change an E account; thus, each column has exactly an A (or ) and an E. In this sense, both the X-operator and the Z-operator ensure that the structure of one A (or ) and one E. The following observation generalizes Lemma 1 for all journal entries.

Observation 2. Under the double-entry system the articulation property of the financial statements ensures the structure of each column must be one of , , , and .

Observation 2 implies that if the financial statements articulate initially after the recognition entry, then the financial statements after the operations (I, X, Z, (X, Z)) should also articulate. However, the interpretations of the “A” and “E” after the operations are subject to the initial state and the operation (or the journal entry) performed.

To illustrate, we provide an accounting explanation for Example 5 in Table 8. The initial state is so that the entanglement property (that is, there are two statements) is satisfied. A sender transmits messages by applying the operators (I, X, Z, or (X, Z)) to the first column and leaves the second account unchanged. The four operations can be thought of in terms of valuation language of accounting: no entry (I), depreciation (X), write-down of the asset (Z), and depreciation followed by an asset write-down (X, Z). (The subscript 1 means the operation is performed on the first column.)

Operation I1 is no journal entry, .

Operation X1 is to depreciate the first asset account, . On the accrual statement, an asset is reclassified as the depreciation expenses so that . The depreciate expense reduces the income by 1 and the accounting identity holds.

Accounting identity

On the cash flow statement, the depreciation expense is non-cash and added back so that (). The cash flow reconciliation identity holds.

Cash flow reconciliation identity

As a result of the X operator, an expense is recorded on the income statement (an “E” on the top statement). On the cash flow statement, there are two items, an (initial) cash expenditure and a non-cash depreciation add-back, so that (an “A” at the bottom statement). The operation X1 ensures the articulation of the financial statements.

Operation Z1 is to write down the first asset account for a positive amount, . On the accrual statement, the losses reduce both the asset balance and the Income account. The accounting identity holds.

Accounting identity

On the cash flow statement, the losses are non-cash and added back directly to Income. Because the asset is revalued from A to , this is a scaling issue which has no impact on either Income or the net change in Cash (. The losses are added back to Income so that the cash flow reconciliation identity holds.

Cash flow reconciliation identity

As a result of the Z operator, the asset on the balance sheet is written downwards (an “” on the top statement). On the cash flow statement, it will still be just the cash expenditure from the initial state (an “E” at the bottom statement). The operation Z1 ensures the articulation of the financial statements.

Operation (X1, Z1) is to first depreciate the first asset followed by a write-down of the asset, . This operation combines both (ii) and (iii). On the accrual statement, the asset is first reclassified as an expense () and then the asset is written down. Collectively, both Income and the asset balance decrease by the amount equal to the sum of the depreciation and the losses. The accounting identity holds.

Accounting identity

On the cash flow statement, the depreciate expense is added back () and the losses are also added back directly to Income.

Cash flow reconciliation identity

As a result of the (X, Z) operation, an expense is recorded on the income statement (an “E” on the top statement). On the cash flow statement, as a combined effect of a cash expenditure and the depreciation add-back (an “A” at the bottom statement). The operation (X1, Z1) ensures the articulation of the financial statements.

More generally, when an asset is revalued, the gains/losses would increase/decrease Income and the asset balance. Since the gains/losses are non-cash, they are directly adjusted to Income on the cash flow statement. The dollar amount of gains/losses won’t affect how much information is transmitted. The receiver obtains four distinct signals (in terms of Income), 0, -1, -losses, and -1-losses; therefore, two-bit channel capacity is obtained.

Proposition 3 can be generalized to a more realistic setting with more than two accounts on the financial statements. The following theorem summarizes the result.

Theorem. One account can transmit two bits of information under the double-entry system with the superposition property when there are accounts and at least two accounts satisfy the articulation property.

The theorem describes the accounting structure under which two bits of information can be transmitted using one account. The two-bit capacity of one account requires (i) at least two accounts; and (ii) at least two accounts (including the first account) satisfy the accounting identity and the cash flow reconciliation identity.

V. Extensions

We consider two extensions to show the robustness of our results. In the first extension, the second column is used to transmit messages. In the second extension, there are more than one account to transmit messages.

5.1. Sending messages using the second account

The two-bit channel capacity result is not constrained by which account is used to transmit messages. Consider a scenario with two financial statements and two accounts in each statement as in Table 10 Example 6. The operations are applied to the second column (so that the subscript is 2).

| Table 10: Example 6—using the second account to transmit messages with two financial statements, EE on the top statement and AA on the bottom statement | Table 10: Example 6—using the second account to transmit messages with two financial statements, EE on the top statement and AA on the bottom statement |
| --- | --- |
|  |  |
|  |  |

The four signals in Table 10 are orthogonal to each other and hence distinct. Four distinct signals convey two bits of information.

Proposition 4. In a scenario with two financial statements and two accounts on each statement, when the second account is used to transmit messages, the two-bit communication capacity is obtained as long as both accounts have the structure of , , , or .

5.2. Channel capacity of the double-entry system with more than two accountings

We are curious whether the channel capacity result can be extended to more accounts. For example, in a structure of two financial statements with three accounts on each statement, how many bits of information can be transmitted if we use the first two accounts? In this section, we generalize our results to a setting with n > 2 accounts.

We provide an illustrative example with three accounts and the first two accounts are used to transmit messages. Three accounts can be represented by an 8-element vector. With three accounts, there can be signals; thus, we consider the following eight operations (messages).

(no journal entry)

(reclassification entry to the first two accounts)

(reclassification entry to the first account only)

(reclassification entry to the second account only)

(revaluation entry to the first account)

((X, Z) to the first account and reclassification entry to the second account)

((X, Z) to the first account only)

(revaluation entry to the first account and reclassification entry to the second account)

The first four operations are X-operators on the first or the second or both accounts. The last four operations are the first four operations augmented by a Z-operator on the first account. As Example 7 in Table 11 shows, all eight signals are distinct and three-bit channel capacity is achieved.

| Table 11: Example 7—using two financial statements and three accounts in each statement to transmit messages) | Table 11: Example 7—using two financial statements and three accounts in each statement to transmit messages) |
| --- | --- |
|  |  |
|  |  |
|  |  |
|  |  |

Proposition 5 generalizes the observation to n-account structure.

Proposition 5. An n-bit channel capacity is achieved under the double-entry system with two financial statements and n accounts on each statement if, and only if, all n accounts satisfy the accounting identity and the cash flow reconciliation identity.

VI. Final Remarks

Double-entry accounting has been around for at least five decades. It has survived almost unimaginable improvements in capturing, processing and communicating information. It is used more widely now than ever before. However, we have very little understanding why double-entry system exists and survives technological innovations and economic advancements with few changes. In this paper, we demonstrate that the double-entry system is an efficient information communication channel. To do so, we proposal a vector representation of the double entry system defined by the accounts and the journal entries. (i) An account is represented by a two-element vector. (ii) Accounts are combined using the tensor products of the vectors. (iii) The reclassification entry and the revaluation entry are represented by the transformation matrices, X-operator and Z-operator. (iv) The signals are distinct as long as the resulting vectors are orthogonal. As discussed in Appendix A, how we frame the double-entry system as a communication channel is consistent with the four axioms in the quantum information theory (Nielsen and Chuang 2004).

We demonstrate that one account can transmit two bits of information in a double-entry system with two financial statements and at least two accounts on each statement. This requires that at least two accounts (including the account that is used for transmitting messages) satisfy (i) the accounting identity, Assets = Equities; and (ii) the cash flow reconciliation identity, the net change in cash equals Income minus the adjustments. It is the salient feature of the double-entry system that both identities are held at any point in time so that the financial statements are articulate. The journal entries are the operators a sender uses to process and transmit information. In contrast to the single-entry system where the net change of Cash is recorded, for journal entries that are non-cash (in particular, the reclassification and the revaluation entries), the reconciliation between Income and the net change in Cash becomes particularly informative and thus determines the information capacity of the double-entry system.

References

Anil, A., J. C. Fellingham, J. C. Glover, D. A. Schroeder, and G. Strang. (Fall 2000). “Inferring transactions from financial statements,” Contemporary Accounting Research Vol. 17 (3): 365-385.

Basu, S. and G. Waymire. (June 2021). “The evolution of double-entry bookkeeping,” working paper. Available at SSRN: http://dx.doi.org/10.2139/ssrn.3093303.

Demski, J. S. (October 1973). “The general impossibility of normative accounting standards,” The Accounting Review Vol. 48 (4): 718-723.

Jensen, M. (April 1983). “Organizational theory and methodology,” The Accounting Review Vol. LVIII (2).

Hatley, R. V. L. (July 1928). “Transmission of information,” The Bell System Technical Journal Vol. 7 (3): 535-563.

Ijiri, Yuji. (1989). Momentum Accounting and Triple-Entry Bookkeeping: Exploring the Dynamic Structure of Accounting Measurement. American Accounting Association, Sarasota, Florida.

Littleton, A. C. (June 1928). “Paciolo and modern accounting,” The Accounting Review Vol. 3 (2), p131-140.

Paton, W. A. (1917). “Theory of the double-entry system,” Journal of Accountancy Vol. 23 (1): p7-26.

Nielsen, M. A. and I. L. Chuang (2004). Quantum Computation and Quantum Information. Cambridge University Press.

Shannon, C. E. (July 1948). “A mathematical theory of communication,” The Bell System Technical Journal, Vol 27 (3): 379-423.

Appendix A

Matrix representation of X-operator and Z-operator

In the text we essentially multiply matrices by vectors in the accounting process where the journal entries explain the changes of the accounts before and after each transaction. To see this, the journal entries are defined by two-by-two matrices and the accounts are defined by two-element vectors.

Define the X-operator and the Z-operator in matrix format, and . Also define the account objects in vector format, , , , and . The reclassification entries (in Definition 2) is written as AX = E and EX = A.

; and

E.

Similarly, the revaluation entries (in Definition 3) is written as EZ = E and AZ = . Note that .

; and

EZ.

Proof of Observation.

It is convenient to prove using the matrix/vector representation. If we start with A, we can reach E, L and R as AX = E, AZ = = L, and AZX = R.

.

If we start with E, we can reach A, L and R as EX = A, EXZ = L, and EXZX = R.

; and

EXZX.

Both X- and Z-operators are square matrices that are its own inverse, and . Moreover, and . We can start with L or R and take the inverse of the operations to reach all the other three accounts. For example, from AZX = R, A can be reached from R.

There are four operators considered in the paper, , , , and . These four matrices are linearly independent and they span the vector space of all the 2x2 matrices. Any 2x2 matrices can be expressed as a linear combination of these four matrices.

This means that any combinations of the X- and the Z-operators can be represented by these four operators.

Q.E.D

Proof of Proposition 1.

For part (i), there are two cases as shown in Tables 1 and 2. For part (ii), there are four cases, two of which are shown in Tables 3 and 4. It is straightforward to show the one-bit capacity if using or to transmit messages. For part (iii), there are four cases, when EA is used to transmit messages, the one-bit capacity is obtained as shown in Table 6. It is straightforward to show the one-bit capacity if using EE, AE or AA to transmit messages.

Q.E.D

Proof of Proposition 2.

In this experiment, the signals are produced by applying the operations to the first account then tensor with the second account. For example, if the initial state is and the X-operator is applied to the first account, then the sum vector is [0 1 1 0].

= =

There are 16 cases in total. If the first column has either two As or two Es. After applying the four operations, three possible signals are produced, , , and ; moreover, and are indistinguishable. Tensoring with the second column that has two As or two Es yields two distinct signals. If tensoring with the second column that has an A and an E, and are indistinguishable; and and are indistinguishable. Again, only two distinct signals are produced.

If the first column has an A and an E, applying the four operations yields four signals, , , , and ; moreover, and are indistinguishable and and are indistinguishable.

If the second account has an E and an A, four distinct signals are produced.

This is because and are distinct or and are distinct. Tensoring the first account with a second account that has an E and an A would create two distinct signals.

If the second account has two As or two Es, only two distinct signals are produced.

That is, and are indistinguishable or and are indistinguishable.

Clearly, only the first column with an A and an E won’t be sufficient because the aggregation (i.e., the sum vector) makes it necessary to tensor the second account. Tensoring the second account with two As and two Es won’t produce four distinct signals.

Q.E.D

Proof of Lemma 1.

“If” part. As discussed in the text, under , an asset is recognized on the balance sheet and a cash expenditure is recorded on the cash flow statement so that . Under , an expense is recognized on the income statement and no adjustment is made on the cash flow statement so that . In both cases, the equality (3) holds.

“Only if” part. Suppose so that an asset is recognized on the balance sheet. There are two possible cases under which the identity (1) holds: either or . From (2), .

In both cases, the cash flow reconciliation identity ensures , meaning there is an adjustment on the cash flow statement. The structure that satisfies (1) and (2) must be .

Suppose there is no adjustment on the cash flow statement (meaning an “A” at the bottom statement). From (2), . From (1), it must be and so that a cash expense is recorded on the income statement. The structure that satisfies both (1) and (2) must be .

A more general statement is to include A, E, L and R.

Results. Under the double-entry system where both the accounting identity and the cash flow reconciliation identity always holds, the structure of the two financial statements and one accounting on each statement must be , , , or .

To see this, the accounting identity implies that Income equals the sum of the changes in Cash and the changes in (non-cash) Assets minus the changes in Liabilities.

The cash flow reconciliation identity states that the net change in Cash equals Income minus the cash expenditures (denoted by ) plus the cash receipts (denoted by ).

Adding the two identities yields

If cash is collected, then the initial structure should be either or in order to achieve the two-bit channel capacity.

Q.E.D

Proof of Proposition 3.

It is immediate from Proposition 2 and Lemma 1. Q.E.D

Proof of Observation 2.

The statement is proved by the illustration in Section 4.2 in the text. Q.E.D

Proof of Theorem.

For N=2, the statement is immediate from Proposition 3.

Prove the statement holds for N=3. The tensor product of three accounts can be obtained by computing the tensor product in order.

The operators apply to the first account. The first account must be either or . If the second account also take the form of either or , then four distinct signals are produced regardless of the format of the third account. For example, , , , are distinct with each other. The first two columns are taken from Table 11.

If the second account takes the form of or , then using the first two accounts yields two distinct signals (see the proof of Proposition 2). However, tensoring the signals with or would yield four distinct signals.

Example A1 demonstrates a scenario with two financial statements and three accounts on each statement. All three accounts satisfy the two identities. There are four distinct signals.

| Example A1: Using the first account to transmit messages with two financial statements, EEE on the top statement and AAA on the bottom statement | Example A1: Using the first account to transmit messages with two financial statements, EEE on the top statement and AAA on the bottom statement |
| --- | --- |
|  |  |
|  |  |

Example A2 demonstrates a scenario with two financial statements and three accounts on each statement. Only the first and the third accounts satisfy the two identities. There are four distinct signals.

| Example A2: Using the first account to transmit messages with two financial statements, EEE on the top statement and AEA on the bottom statement | Example A2: Using the first account to transmit messages with two financial statements, EEE on the top statement and AEA on the bottom statement |
| --- | --- |
|  |  |
|  |  |

Parallel analysis applies to the case of N>3. The first account always takes the form of either or . As long as there is another account taking the form of either or , the two-bit channel capacity is obtained.

Q.E.D

Proof of Proposition 4.

Suppose the second account is used to send messages. Consider an example in which an X-operator is applied to the second account and the initial state is and the sum vector is [0 1 1 0].

| = = |
| --- |

The parallel logic from the proof of Proposition 2 applies to support the statement.

Q.E.D

Proof of Proposition 5.

We prove by induction. The statement is true for n = 2 (see Proposition 3).

Suppose the statement is true for n = k. That is, in a structure with k accounts, the sender uses the first (k-1) accounts to transmit messages. There are distinct signals produced and therefore bits of information are transmitted as long as all k accounts satisfy both identities.

For n = k+1, we construct distinct signals. The first k accounts, if having an E and an A, can produce distinct signals. Denote these signals by , where “CS” is cash flow statement and “AS” is accrual statement. Switching the account between the top and the bottom statements would yield another signals, written as . However, and are indistinguishable. Tensor the (k+1)th account with the first k accounts. Applying the logic from the proof of Proposition 2, there are two possible cases depending on the property of the (k+1)th account.

If the (k+1)th account has an A and an E, then and are distinct; or and are distinct. In this case, we produce distinct signals.

If the (k+1)th account has two As or two Es, then then and are indistinguishable; or and are indistinguishable. In this case, we produce distinct signals.

In the first case, both the accounting identity and the cash flow reconciliation identity are maintained for the (k+1)th account.

Q.E.D

Appendix B—A comparison of double entry accounting and quantum information

Nielsen and Chuang (2004) list four axioms of quantum information. They are briefly described below alone the corresponding property of accounting.

Qubits (Quantum bits). The object of interest are represented by the two-element vectors consisting of a one and a zero: [1 0] and [0 1].

Accounts, A and E, are the accounting analogs.

Quantum operations are linear operators which transform quantum objects.

: bit of flip operator

: phase flip operator

The journal entries, not coincidentally labeled X and Z, perform the same linear function in the accounting setting.

Qubits are combined into a larger system using tensor multiplication, just as in the accounting development.

The measurement axiom specifies how qubits with any vector orientation are observed. In the accounting development we restrict attention to the end points: (1) when vectors are scalar multiples (indistinguishable signals); and (2) orthogonal vectors (distinguishable signals).

We don’t confront other than the special cases, and, hence, are able to avoid difficulties like the collapse of the wave function, and paradoxes such as “Schrodinger’s cat.”

Derived quantum properties.

Superposition—qubits can exist in more than one state at a time. That is, the vectors [1 0] and [0 1] can simultaneously describe the state of a single qubits. In the accounting realm, an account can have different representations in different financial statements. The existence of accrual statements (balance sheet and income statement) provides the ability to report the same account in different ways.

Entanglement—entangled qubits are defined as a system which cannot be produced by tensor multiplication. [1 0 0 1], one of the Bell states, is an example. Entanglement is a powerful information processing tool; the information processing behavior of a qubit outside of the experimenter’s reach can be controlled by manipulating the qubit accessible to the experimenter. This is what Einstein referred to as “spooky action” at a distance. The accounting identities ensure the accounting reports have an entanglement property. For example, cannot be constructed from tensor multiplication of two accounts. It is analogous to a Bell state. It possesses at least some of the information processing ability of a Bell state. That is, the amount of information carries by one account is increased even when the other entangled account is not manipulated at all.

## Footnotes

- footnote 1: Hartley (1928) proposes a measure, later called entropy, to quantify the rate of information transmission for a system. Shannon (1948) describes a communication system consisting of five parts, an information source that produces a message, a transmitter that produces a signal by encoding the message, the channel that transmits the signal, a receiver who decodes the signal, and the destination person for whom the message is intended. The accounting system comprised of T-accounts and journal entries is a communication system in an economic context. The manager decides to undertake some economic transactions based on some private information (the information source). Transactions are transmitted using journal entries (transmitter) and recognized in the financial statements. A receiver decodes the signal embedded in the financial statements to inform the decision-making process.
- footnote 2: We borrow the term “superposition” from quantum information theory. In Appendix B, superposition is explained as one of the axioms in quantum information theory; any quantum state can be represented by a two-element vector.
- footnote 3: In a chart of accounts, there are five types of accounts, assets (A), liabilities (L), equities, revenues (R) and expenses (E). We consider four types in our framework, A, L, R and E. Equities, which include contributed capital and retained earnings, are represented indirectly. Contributed capital can be represented by the liability vector (L = [0 -1]) because both represent claims/ownership of recognized assets. Retained earnings are accumulated earnings and the change of retained earnings can be represented by the revenue and/or the expense vectors (R = [-1 0] and E = [1 0]).
- footnote 4: The vector representation of the accounting objects helps formulate how information is processed by the accounting system in a way that is consistent with the information theory. Similar to telegraphy where messages are encoded and transmitted by dots and dashes, in accounting the managers’ messages (transactions or journal entries) are encoded and transmitted by accounts (signals).
- footnote 5: It is possible that a recognition entry does not involve cash, for example, acquiring an equipment with a loan (Debit Equipment Credit Long-term Debt). This transaction can be journalized as two cash-based entries: first, borrowing cash (Debit Cash Credit Long-term Debt), and second, using the borrowed cash for acquisition (Debit Equipment Credit Cash).
- footnote 6: The X and the Z operators are Pauli matrices; the matrix representations are provided in Appendix A.
- footnote 7: By Assumption 1 and for expositional convenience, we consider the magnitude of 2 for the revaluation entries. For example, when an asset is revaluated downwards by 2, the asset changes from a debit balance to a credit balance. A gain/loss account arises to maintain debits equal credits. To define Z, we do not include the gain/loss account as they are not essential in deriving our main results.
- footnote 8: In a directed graph representation of the accounting system (e.g., Arya et al., 2000), accounts are the nodes, and journal entries are the directed edges—each edge pointing from the credit account (tail) to the debit account (head). Observation 1 implies that an edge between two non-cash accounts can be represented by a combination of the X and the Z operators.
- footnote 9: Any other combinations of X and Z operations would be equivalent to one of these four operations. To see this, note that both the X-operator and the Z-operator are reversible. An even number of X-operators (or Z-operators) is equivalent to an I-operator (e.g., or ); and an odd number of X-operators (or Z-operators) is equivalent to an X-operator (or Z-operator) (e.g., or ). (X, Z) and (Z, X) yield signals that are in the same subspace, which means that (X, Z) and (Z, X) yield indistinguishable signals.
- footnote 10: In general, the number of bits is the log base 2 of the number of signals; and hence bits.
- footnote 11: In an alternative setting, cash is initially received and either a revenue or a liability is recognized. Our analysis and findings remain qualitatively and quantitatively the same if initially L or R is recognized.
- footnote 12: The two-row structure can be produced by applying two operations such as (X+Z) on an account—one vector yields two vectors. For example, performing (X+Z) on E is to apply X to E on the top row and apply Z to E at the bottom; is produced. To get a vector representation of the resulting signal, we add up the two vectors and the sum vector is [1 1]. For another example, performing (I+X) on E is to apply I to E on the top and to apply X to E at the bottom; the resulting signal is and the sum vector is [1 1].
- footnote 13: A tensor product of two two-element vectors is a four-element vector, written as
- footnote 14: The tensor product of three vectors can be computed as .
- footnote 15: The following quote from Jensen (1983) still accurately characterizes our state of knowledge about double-entry accounting.“The usefulness and power of double-entry bookkeeping is testified to by its survival since at least the 15th century and its continuing wide-spread use. Viewing double-entry bookkeeping this way leaves me believing that we still do not thoroughly understand why it is a powerful organizing device. I am so used to thinking of assets and the claims on them, equities and liabilities, as a way of organizing thoughts about companies that it is hard to conceive of alternatives.”
