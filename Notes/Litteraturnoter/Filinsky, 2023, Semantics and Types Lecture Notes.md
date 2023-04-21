# Chapter 1
Semiformal proof = written in real language, based on formal
## Syntax and semantics
### sorts
Sort = kinda like sets but countable (like a type)
Examples: number, identifiers, phrases
Sorts are non-empty

### Operations and terms
Operators have source sorts and output sorts
Syntactic constructors act as operators (example: if is an operator that takes a boolean expression and two commands and returns a command)
Operators are often overloaded (+ works for integers and real numbers for example)
Term = either parameter value OR function applied to some arguments
Terms belong to a sort
Triple equal sign means macro-like assignment for abbrevity
### Predicates and formulas
predicate takes sorts of specific types and denote some kind of truth
Predicates build up a formula
examples: predicate could be <=
formula could be a <= n
Compound formulas connect atomic formulas with AND, OR and so on.
=> is right-associative

## Proof structure
A proposition consists of some (sub)sets of variables of some sort, assumptions and conclusions
Assumptions and conclusions must not contain any free variables beyond the parameters

![[Pasted image 20230130220707.png]]

If we can check all hypothesis and the conclusion for all variables, then we know if the proposition is _true_. If one sort is infinite, then we need to prove instead.

Sequent, consequent judgment = the notion of provability
Formulas = antecedents
consequent
![[Pasted image 20230130221206.png]]

A proof is an argument given that no matter the parameters, if the antecedents hold, then the consequent holds as well

A proposition supported by a proof is called a theorem

If proof rules are sound, we can only proof true propositions

![[Pasted image 20230130221628.png]]
Top parts are called premises, bottom is called conclusions

Axioms involve no premises
The assumption axioms says that if $\Gamma$ contains $Q$ then $\Gamma\vdash Q$ 
![[Pasted image 20230130222610.png]]

You instantiate a rule by replacing metavariables, example:

![[Pasted image 20230205134821.png]]

Elimination:
![[Pasted image 20230130223602.png]]

## Presentation styles of proofs
forward presentation (post-order): Having shown ... and ... we now conclude

Backward (or goal-directed) presentation (pre-order): In order to show ..., we only need to show ... and ...

# Proof rules
Assumption rule:
![[Pasted image 20230130224258.png]]
Axiom:
![[Pasted image 20230130224642.png]]
Lemma:
![[Pasted image 20230130225035.png]]
![[Pasted image 20230131221120.png]]
![[Pasted image 20230131221139.png]]
![[Pasted image 20230130225612.png]]
![[Pasted image 20230130225625.png]]
![[Pasted image 20230130230141.png]]
![[Pasted image 20230130230154.png]]
![[Pasted image 20230131203907.png]]
![[Pasted image 20230131214527.png]]

![[Pasted image 20230131204217.png]]
![[Pasted image 20230131204233.png]]
![[Pasted image 20230131205158.png]]
![[Pasted image 20230131205212.png]]
![[Pasted image 20230131213225.png]]
![[Pasted image 20230131213239.png]]
![[Pasted image 20230131213254.png]]
![[Pasted image 20230131213310.png]]
![[Pasted image 20230131214800.png]]
![[Pasted image 20230131214920.png]]
![[Pasted image 20230131215010.png]]
![[Pasted image 20230131215250.png]]

# Chapter 2

## Big-step IMP semantics and simple reasoning
### Recapitulation of the IMP Language
![[Pasted image 20230208110305.png]]
![[Pasted image 20230208111350.png]]
![[Pasted image 20230208111638.png]]

## Inductive reasoning about IMP Semantics
