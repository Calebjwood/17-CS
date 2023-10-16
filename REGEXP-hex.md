## REGEXP - Matching a Hex Value
This gist will explain a regular expression that is used to match hex vaules

## Summary

We are gonna break down and explain the expression :

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
Anchor:^

code used: /^#

this anchor indicates that the string must start with #

anchor: $/

code used:

this anchor indicates that the 3 characters before the $ have to match the 3 last charachters of the string 

### Quantifiers

Quantifier: ?

code used: /^#?

? is equal to setting a boolean the the character before the siqn

Quantifer: {}

code used: [a-f0-9]{6} | [a-f0-9]{3}

indicated that the REGEXP will only allow 6 characters between A - F, and 0 - 9. the same being for the second bracket but that line will only allow 3 characters
the | symbol is the OR sign and is saying that we will only allow 6 charactors defined be the first bracket or 6 characters defined by the second bracket
### Grouping Constructs

grouping:()

code used: ([a-f0-9]{6}|[a-f0-9]{3})

anything inside of the () is treated as a single set of characters so that the following character can act on all the characters inside of the ()

### Bracket Expressions
bracket expression: []

code used: [a-f0-9]

the [] is used to match the characters to the characters indicated inside of the bracket

### Character Classes

code used: a-f0-9

this code says we will only allow characters between those values

### The OR Operator

OR operator: |

code used:[a-f0-9]{6}|[a-f0-9]{3}

the | symbol is the OR sign and is saying that we will only allow 6 charactors defined be the first bracket or 6 characters defined by the second bracket


## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)