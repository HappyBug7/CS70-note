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
The **Contrapositive** of "$P\Rightarrow Q$" is "$\lnot Q\Rightarrow \lnot P$"
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

# Lecture 2
*Proofs*
## Ways to prove
- By Example
- Direct
- By Contraposition ($P\Longrightarrow Q\equiv\lnot Q\Longrightarrow\lnot P$)
- By Contradiction ($P \text{ and } \lnot P$ cannot happen at the same time)
- By Cases

## Quick Background and Notation
- Intigers closed ubder addition (*$a,b\in Z\Longrightarrow a+b\in Z$*)
- "$a|b$" means "$a$ divides $b$"
	- **Formally:** $a|b\Longleftrightarrow \exists q\in Z, b=aq$

## Direct Proof
**Theorem:** For any $a,b,c\in Z$, $\color{blue} \text{if }a|b \text{ and }a|c\text{ then }a|(b-c)$
**Proof:** Assume $a|b$ and $a|c$
then $b = qa$, $c = q'a$
$b-c = (q-q')a$, $(q-q')$ by defination is an integer, then
$a|(b-c)$
Direct Proof Form:
- Assume $P$
- ...
- Therefore $Q$

## Proof by Contraposition
**Thm:** For $n\in Z^{+}$, and $d|n$, If $n$ is odd then $d$ is odd
**Goal:** Prove $P\Longrightarrow Q$
- Assume $\lnot Q$
- Prove $\lnot P$
$\lnot Q:$ $d$ is even
$\lnot P:$ $n$ is even
**Proof:** Assume $d$ is even, $d|n$
then $n = qd$ is even, $\lnot P$ proved
$\lnot Q\Longrightarrow\lnot P\equiv P\Longrightarrow Q$

## Proof by Contradiction
**Thm:** $\sqrt2$ is irrational
To prove this, we must show: For every $a,b\in Z$, $\left(\frac{a}{b}\right)^{2}\neq2$
**Goal:** $P$
- Consider $\lnot P$
- Prove $\lnot P\Longrightarrow \text{False}$
- then the contraposition: $\text{True}\Longrightarrow P$, i.e. $P$ is always True
$\lnot P:$ $\sqrt2$ is rational ($\sqrt2 = \frac{a}{b}, \text{ for }a,b\in Z$)
Therefore $a=\sqrt2b$, $a^{2}=2b^{2}$
then $a^{2}$ is even, $a$ is even: $a=2k$
then $b^{2}=2k^{2}$, $b$ is even
$a$ and $b$ have a common factor, contradiction!
then $\text{True}\Longrightarrow P$

**another example:**
**Thm:** There are infinitely many primes
**Proof:**
Assume there are finitely many primes: $p_{1},p_{2}, ...,p_{n}$
then consider $q = 1+\prod\limits^{n} p_{i}$
since $q$ is larger than any prime, $p_{i}|q$
also $p_{i}|\prod\limits^{n}p_{i}$
then $p_{i}|q-\prod\limits^{n}p_{i}=1$, i.e. $p_{i}\leq1$ contradiction!
therefore there are infinitely many primes


