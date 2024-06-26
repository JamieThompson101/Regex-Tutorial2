## Regex Tutorial
A REGEX is a regular expression that searches for matching values/patterns within a string. The following REGEX is an example that looks for the string to match the general makeup of an email address.

## Summary

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
This regex tutorial will explore the regex of matching an email addressFor this regex, each component has a specific responsibility to make sure or verify that the user enters an email address in the correct format which in this case begins with characters followed by @ symbol and, lastly, the domain.\

## Table of Contents
*Anchors

*Quantifiers

*Character Classes

*Flags

*Grouping and Capturing

*Bracket Expressions

*Greedy and Lazy Match

*Boundaries

*Back-references

*Look-ahead and Look-behind

*Author

## Anchors

Anchors are what starts and ends the regular expression. In this email code,

/^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/,

the anchors are the ^ and the $. This code is telling the computer that we are looking for strings that starts with

^([a-z0-9_.-]+)

and end with

.([a-z.]{2,6})$.

Therefore, it must begin and end with the given parameters within the code. otherwise, it is not a match.

## Quantifiers

The example REGEX includes the following quantifiers: + which is used to match one or more of the preceding token {2,6} which matches the specified quantity of the previous token, in this case between 2 and 6 characters. Alternatives would be {2,6}, which looks for 2 digits exactly, or {2,4} which looks for 2 or more characters.

## Character Classes

Character Classes distingush specific kinds of characters from a certain set. Regex has character classes: \. and \d. The . means any character except a line break. By placing a backslash \ in front of the ., it's "escaping" the character and is taken literally. The \d matches any single digit equivalent to [0-9].

An example of \.: in the expression a\.c, it matches a.c. The . is taken literally - as period.

## Flags

The example REGEX utilizes is the following flags: g which stands for global search.

## Grouping and Capturing

The example includes the following group: ([a-z0-9_\.-]+), this expression includes + which means we match at least one or more of any characters in the square brackets [a-z0-9_\.-]. a-z is lowercase letters from a to z, 0-9 is numbers from 0 to 9, _ is underscore, \. is period, and - is hyphen.

## Bracket Expressions

Bracket expressions are used to specify characters to match, they are enclosed in square brackets[]. Our regex has three bracket expressions: ([a-z0-9_\.-]+), ([\da-z\.-]+), and ([a-z\.]{2,6}).

An example of bracket expressions: in the expression [abc], it matches any character in the brackets; either a or b or c.

## Greedy and Lazy Match

In the given code for matching an email, there isn't a greedy or lazy match included.

## Boundaries

The metacharacter \b is an anchor like the caret and the dollar sign. It matches at a position that is called a “word boundary”. This match is zero-length.

## Back references

A backreference in a regular expression identifies a previously matched group and looks for exactly the same text again. A simple example of the use of backreferences is when you wish to look for adjacent, repeated words in some text. The first part of the match could use a pattern that extracts a single word.

## Look-ahead and Look-behind

Lookahead and lookbehind, collectively called “lookaround”, are zero-length assertions just like the start and end of line, and start and end of word anchors explained earlier in this tutorial. The difference is that lookaround actually matches characters, but then gives up the match, returning only the result: match or no match. That is why they are called “assertions”. They do not consume characters in the string, but only assert whether a match is possible or not. Lookaround allows you to create regular expressions that are impossible to create without them, or that would get very longwinded without them.

## Author 

Visit my github link if you have any questions, comments, or simply just want to see my work: https://github.com/JamieThompson101/-Regex-Tutorial2
