# Matching URLs using a Regular Expression (Regex Tutorial)

In this tutorial we will be working with this expression: 

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

I will attempt to guide you through what all of these apparently random charaters mean, and why it is useful for developers.

## Summary

As stated above, this tutorial will (hopefully) concicely describe and explain the importance of validation of a URL using a regular expression. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

# Regex Components
If you are anyrthing like me, your first impression of a regular expression(Regex) was that it is just a bunch of gibberish. While that may be true, it really is just a complex string of what are called "Regex Components" with each component serving a specific purpose. We will go over each individual component in detail below.
## Anchors

Two examples of anchors are the symbols `^` and `$`. The `^` anchor is useful because it denotes a string that begins with the exact characters that follow it.  For example, a `^` followed by a string containing "chicken nuggets" will specically look for "chicken nuggets." Regex are case sensitive, however, so if the text was "Chicken Nuggets," there would not be a match. `$` is very similar to `^`, but it reads characters that precede it.  Meaning, `$` is useful at the end of the expression. 

## Quantifiers
Quantifiers determine how many of the same character or group of characters must be present to be considered a match. One example of a quantifier is `*`. This is a quantifier that matches the preceding character zero or more times. What this means is in your expression if you had `b70*j4*`, the `*` quantifier is looking for a `0` and a `4`. This is useful because it is essentially a boolean on if the numbers `0` and `4` are in the given URL the regex is trying to validate. Another quantifier is `+`. This quantifier is different than a `*` quantifier because it will look for one or more characters that precede it. This quantifier would be useful for trying to verify specific words, or words with similar letters in the same order.  
## Grouping Constructs
Before we dive in to Grouping Constructs, we first need to learn what a subexpression is. A subexpression is a part of a larger expression that individually is an expression itself. A great example of a subexpression is "www." This is individually an expression, but it is commonly used in larger expressions "www.google.com" for example. Grouping Constructs characterize the subexpressions of a regular expression and find matches of the given string.
## Bracket Expressions
A bracket expression is an expression bookended by brackets "[]." This will match any characters inside the brackets.  It is more of a specific search due to it looking for specific character(s).
## Character Classes
Character classes, also called character sets are combinations of characters that serve a specific function. one of the simplest examples of a character class is `a-d`. This character class looks for a, b, c, and d. Another example is `/d`, which will look for any digit in a given string.
## The OR Operator
The OR operator, or the common operator, is signified with `|`. The significance of the OR operator is that it accepts matching strings preceding and following the `|`.
## Flags
A flag is a parameter in a regex that changes the way it searches.  Examples of how flags change the parameters of the search are, making an expression ignore casing (`i`), making anchors match the beginning and ending of a line rather than a string (`m`), making the character `.` match newlines (`s`), etc. You can think of flags as changing the filter of how anchors, quantifiers, and regular expressions in general work.
## Character Escapes
Character escaping is a fairly simple concept compared to the ones above.  This idea is to negate special characters that would otherwise have meaning in a regex. For example, to make a `^` act as a normal part of a string and not an anchor would be done by saying `\^`. This negates the caret and treats it as a string rather than a character with a specific function.
# Author
This regex tutorial was written by Cole Carter. Here is my GitHub profile link if you are interested in seeing more of my work: https://github.com/ColeCarter9530
