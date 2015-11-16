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


http://www.cs.rochester.edu/~nelson/courses/csc_173/proplogic/expressions.html

## Operator Precedence(#Operator-Precedence)

There is no natural order of precedence among logical operators

The general rule is inside out if in nested parentheses and left to right.
There also a general rule about the order of precedence being
1 Negation
2 And
3 Or


For the sake of removing a lot of parentheses some people set arbitrary
precedence between logical operators.

a language is a formal languages if operator precedence is defined.
a formal language also must be [functionally complete](#https://en.wikipedia.org/wiki/Truth_function#Functional_completeness).


arbitrary order taken from [wikipedia](#https://en.wikipedia.org/wiki/Logical_connective#Order_of_precedence)

|Name            |  precedence |
|Negation        |  1          |
|And             |  2          |
|Or              |  3          |
|Implication     |  4          |
|Bi-Implication  |  5          |

a different set of precedence that includes parentheses

| operators | precedence |
| () | 1 |
| \neg | 2 |
| And Or Xor | 3 |
| Implication Bi-Implication | 4 |

When trying to find the "right" order of precedence I was going to base it on programing languages,
they also have slightly different rules. I have not found one that break the NOT,AND,OR rule.

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


## References(#References)
https://en.wikipedia.org/wiki/Truth_function#Functional_completeness
https://en.wikipedia.org/wiki/Propositional_calculus
https://en.wikibooks.org/wiki/Discrete_Mathematics/Logic
http://www.cs.rochester.edu/~nelson/courses/csc_173/proplogic/expressions.html
https://en.wikipedia.org/wiki/Truth_function#Arity
