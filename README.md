# REGEX Tutorial

Hello! This is a helpful guide on how to utilize Regular Expressions (Regex) and break down the individual components that make up a regex expression.

## Summary
For this tutorial we are going to analyzing this regex expression for matching an email:
``` md
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```

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
Anchors are characters that singal the start and end of an expression. These characters are:
* `^` Which signifies the beginning and
* `$` Which signifies the end

An example of this can be found at the beginning and the end of the expression
### Quantifiers
Quantifiers set limits to strings or individual sections of strings. This often includes a minimum and a maximum number of characters. Examples of these kind of quantifiers are:
* `{ x }` Matches the pattern exactly x number of times
* `{ x, }` Matches the pattern at least x number of times
* `{ x, y }` Matches the pattern a minimum of x times and a maimum number of y times 

An example of this can be found at the end of the sample regex. Some other examples of quantifiers include
* `*` Matches the pattern zero or more times
* `+` Matches the pattern one or more times
* `?` Matches the pattern zero or one time
### Grouping Constructs
Grouping Constructs are the primary way of containing subexpressions. The way this is expressed is though `()`

You can see this put to use in the sample regex.
### Bracket Expressions
Bracket expressions that use [] as a way to represent a range of characters. This is represented in the following expressions:
* `[a-z]` The string can contain any lowercase letter between a-z. 
* `[A-Z]` The string can contain any uppercase letter between a-z. 
* `[0-9]` The string can contain any number between 0-9. 
* `[_-]` The string can contain any non-alphanumeric characters. 

You can find examples of all of these in the following portions of the sample regex code :
``` md
[a-z0-9_\.-] [\da-z\.-] [a-z\.]
```
### Character Classes
Character classes define sets of characters. One example of the classes are the bracket espressions we just covered!
### The OR Operator
The OR Operator allows the use of grouping multiple constructs using the `|`
### Flags
Flags are placed after the second slash as a way to define additional functionality.
### Character Escapes
To put it simply, `\` in a regex expression escapes a character that would otherwise be interpreted literally
## Author

Payne Kerz

paynekerz@gmail.com

[Github](https://github.com/paynekerz)
