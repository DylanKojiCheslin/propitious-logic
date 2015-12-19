# propitious-logic
Study of propositional logic
that will be made into JavaScript library



[overview](#prop-logic-overview)
[Propositional State](#Propositional-State)
[Propositional Variables](#Propositional-Variables)
[Logical Operators](#Logical-Operators)
[Operator Precedence](#Operator-Precedence)
[Compound Proposition](#Compound-Proposition)
[Examples](#example-props)
[References](#References)

## overview (#prop-logic-overview)

Propositional Logic is the study of truth of statements and the relation of the
truth between statements.

## Propositional State(#Propositional-State)

A single entry on a Truth Table: true/false, 0/1

## Propositional Variables(#Propositional-Variables)

Named Letters ex: (pqrs)
both T/F in both Propositional States



## Logical Operators(#Logical-Operators)
an incomplete list of operators


Negation
And
Or
Implication
Bi-Implication
Nand
Xor
Nor

a functionally complete set of operators can be used to
express all possible truth tables[functionally complete](#https://en.wikipedia.org/wiki/Truth_function#Functional_completeness).

http://www.cs.rochester.edu/~nelson/courses/csc_173/proplogic/expressions.html

## Operator Precedence(#Operator-Precedence)

The general rule is inside out if in nested parentheses and left to right.
There also a general rule about the order of precedence being
1 Negation
2 And
3 Or


To remove a lot of parentheses some people set arbitrary precedence between logical operators.

arbitrary order taken from [wikipedia](#https://en.wikipedia.org/wiki/Logical_connective#Order_of_precedence)

|  precedence |Name            |
|  1          |Negation        |
|  2          |And             |
|  3          |Or              |
|  4          |Implication     |
|  5          |Bi-Implication  |

a different set of precedence that includes parentheses

| precedence | operators                  |
| 1          | ()                         |
| 2          | \neg                       |
| 3          | And Or Xor                 |
| 4          | Implication Bi-Implication |

It would be interesting to try to have a compile time injection of the order of precedence.
There may be something to operators precedence being based on how often the operator are in a functionally complete set.

the number of props a logical operator takes is know as its [Arity](#https://en.wikipedia.org/wiki/Truth_function#Arity)

## Compound Proposition(#Compound-Proposition)

Compares 0 or more
(Propositional Variables), (Propositional States) or (Compound Propositions)
by a logical operator and returns a Propositional State.

0 or more PropVar/PropState/CompoundProp
1 logical operator

in the majority of cases your using 1 or 2 Propositions in a compound
such as:
Negation of p
p and q
r or s

## Examples(#example-props)

Examples:

2 + 2 = 4 and 3 * 3 = one million

example 1.

the statement (2 + 2 = 4) will be called p

the statement (3 * 3 = one million) will be called q

the propositional state of p is true

the propositional state of q is false

this statement can be written as:
p ^ q
p AND q

## Features
the library should be able to take a propositional statement
return a truth table
tell if the statement is boolean satisfiable

## References(#References)
https://en.wikipedia.org/wiki/Truth_function#Functional_completeness
https://en.wikipedia.org/wiki/Propositional_calculus
https://en.wikibooks.org/wiki/Discrete_Mathematics/Logic
http://www.cs.rochester.edu/~nelson/courses/csc_173/proplogic/expressions.html
https://en.wikipedia.org/wiki/Truth_function#Arity
