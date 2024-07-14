# Lecture 1
## The language of proofs
- Propositions
- Propositional Forms
- Implication
- Truth Tables
- Quantifiers
- More De Morgan’s Laws

## Propositions
*Statements that are true or false.*
![[Pasted image 20240714165313.png]]

## Proposition Forms
*put propositions together to make another*
- Conjunction ("and"): $P\wedge Q$
	- $P\wedge Q$ is True when both $P$ and $Q$ are True
- Disjunction ("or"): $P\vee Q$
	- $P\vee Q$ is True when at least one $P$ or $Q$ is True
- Negation ("not"): $\lnot P$
	- $\lnot P$ is True when $P$ is False

## Truth Tables for Popositional Forms
![[Pasted image 20240714171324.png]]
$\lnot(P\wedge Q)\equiv \lnot P\vee\lnot Q$
$\lnot(P\wedge Q)\equiv \lnot P\vee\lnot Q$ *DeMorgan's Law for Negation: distribute and filp*

## Implication
$P\Rightarrow Q$ interpreted as
if $P$, then $Q$

## Non-Consequences/consequences of implication
The statement "$P\Rightarrow Q$"
only is False if $P$ is True and $Q$ is False
$P\Rightarrow Q$ and Q are True does $\color{red}{\text{not}}$ mean $P$ is True
$P\Rightarrow Q$ and $P$ are True does mean $Q$ is True
i.e.: $((P\Rightarrow Q)\wedge P)\Rightarrow Q$ *use propositional formulas to describe implication*
crazy fact: $\lnot P\vee Q \color{red}\equiv \color{black}P\Rightarrow Q$

## Contrapositive
The **Contrapositive** of "$P\Rightarrow Q$" is "$Q\Rightarrow P$"
**Logically equivalent** Notation: $\equiv$
$P\Rightarrow Q\equiv \lnot P\vee Q\equiv \lnot(\lnot Q)\vee \lnot P\equiv \lnot Q\Rightarrow \lnot P$



