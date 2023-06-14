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

## Anchors

Two examples of anchors are the symbols `^` and `$`. The `^` anchor is useful because it denotes a string that begins with the exact characters that follow it.  For example, a `^` followed by a string containing "chicken nuggets" will specically look for "chicken nuggets." Regex are case sensitive, however, so if the text was "Chicken Nuggets," there would not be a match. `$` is very similar to `^`, but it reads characters that precede it.  Meaning, `$` is useful at the end of the expression. 

## Quantifiers

## Grouping Constructs

## Bracket Expressions

## Character Classes

## The OR Operator

## Flags

## Character Escapes

# Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
