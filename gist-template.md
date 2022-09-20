# Regular Expressions (Regex) Tutorial
## What is a Regex?
"Regular Expressions," or "Regex," is a sequence of special characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be:
-used to find certain patterns of characters within a string
-used to find and replace a characted or sequence of characters within a string 
-used to validate input

For example, the following regular expression can be used to verify that user input is a valid email address:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

Each component of this regex has a unique responsibility to make sure that a user enters an email address that begins with an unspecified number of characters preceding the `@` symbol, followed by a domain.
## Summary 

In this tutorial, I will explain what different component parts do for a specific regex. 

For the purposes of this demonstration, I will break down "Matching a Hex Value" regex to obtain a better understanding of regular expressions and their components.

Matching a Hex Value: `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

## Table of Conetents 
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Bracket expressions](#bracket-expressions)
- [Character classes](#character-classes)
- [OR operator](#OR-operator)
- [Author](#author)

## Anchors

`/^`#?([a-f0-9]{6}|[a-f0-9]{3})`$/`

The "Matching a Hex Value" we're reviewing uses two anchors, ^ and $. Anchors are used at the start and end of a string or expression.
- The ^ anchor signifies that the string begins with the character that follows it. For this regular expressins, the starting character is #.
- The $ anchor signifies a string that ends with the character that precedes it.

## Quantifiers

/^#`?`([a-f0-9]`{6}`|[a-f0-9]`{3}`)$/

Quantifiers set the limits of a string or expression, it lets us know how many characters are expected. Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. If the "*,+,?,{}"* characters are found within regular expressions, they are considered quantifiers. The "Matching a Hex Value" has the following quantifiers. 
- The ? indicates the expression to match 0 or 1 time
- The {6} and {3} indicates that the length of the component preceding these quantifiers should be 6 for `{6}` and 3 for `{3}`

## Bracket Expressions

/^#?`([a-f0-9]{6}|[a-f0-9]{3})`$/

Bracket expressions in our regular expression signify the beginning of a character class or quantifier statement. In our example, we use parenthesis to define our bracket expressions.

## Character Classes

/^#?(`[a-f0-9]`{6}|`[a-f0-9]`{3})$/

 Character classes are components within our regular expression that tells us what type of characters to expect. In our example our character classes are confined within brackets `[]`. The "Matching a Hex Value" has the following two character classes -  `[a-f0-9]` and `[a-f0-9]` which searches for the same values.
 - `a-f` searches for letters *a-f*
 -  `0-9` searches for digits *0-9*

## OR Operator

/^#?([a-f0-9]{6}`|`[a-f0-9]{3})$/

 The "or" operator within a regular expression is defined using the `|` element. The "or" operator indicates that it could be one or the other of the two components we are separating with the `|` symbol.  For this example, we have ([a-f0-9]{6}`|`[a-f0-9]{3}). The "or" operator separates these 2 components. This means that our hex value could either be 6 characters `[a-f0-9]{6}` or 3 characters `[a-f0-9]{3}`.

## Author

Jennyfer Constanza

This tutorial is brought to you by Quality Assurance Specialist, Jennyfer Constanza. 
GitHub: [JennyferConstanza](github.com/jennyferconstanza)