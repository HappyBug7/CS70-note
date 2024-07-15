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


## Converse
Converse of "$P\Rightarrow Q$" is "$Q\Rightarrow P$"

## Defination
$P$ i.i.f. $Q$, $P\Longleftrightarrow Q$ (*notataion: "$\Longleftrightarrow$" stands for "Logically equivalent"*)

## Variables
The follow statements
- $\sum\limits_{i=1}^{n}i=\frac{n(n+1)}{2}$
- $x>2$
- $n$ is even and the sum of two primes
Are they **propositions**?
No! Because they have free variables
We can call them predicates, same as boolean valued functions from **61A**

## Quantifiers
Consider the proposition: "For all natural numbers $n$, $\sum\limits_{i=1}^{n}i=\frac{n(n+1)}{2}$"
propositions has universe: "The natural numbers".
Universe examples incude:
- $\mathbb{N}=\{0,1,...\}$
- $\mathbb{Z}=\{...,-1,0,...\}$
- $\mathbb{Z^{+}}$ (positive integers)
- $\mathbb{R}$ (real numbers)
- Any set..
In English: “the square of every natural number is a natural number.”
$(\forall x \in N)(\exists y\in N)(y=x^{2})$
English: there is an x in S where P(x) does not hold. That is,
$\lnot(\forall x\in S)(P(x))\Longleftrightarrow(\exists x\in S)(\lnot P(x))$

