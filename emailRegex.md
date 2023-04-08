# Regex Email Tutorial

A regex, which is short for regular expression, is a sequence of characters that defines a specific search pattern. They are used to validate input such as email.

## Summary

Regex code that is used is: 

``/^[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+@[a-zA-Z0-9-]+(?:\.[a-zA-Z0-9-]+)*$/.``

Using the pattern(s) above you can validate such things as emails or phone numbers. You can use regex to find patterns for emails where anything before an '@' symbol is the username and anything after is the domain [asdf]@[domain.name]. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)

## Regex Components

### Anchors

Anchors don't match any characters. There are instead used to match a position either before, after or between characters. The characters used for anchors are ^ - for the start of a string or $ - for the end of a string. Example:

The regex ^abc matches abc but a^bc does not match because b is not the start of the string.

The regex \$c matches c in abc because the c is the last character of the string. $a does not match because it is not at the end.

### Quantifiers

Quantifiers match a number character, group, or character class in a string. It is used in the curly brackets { } that sets a minimum and maximum limit. Example:

{2,6} - This indicates that the string needs to be a minimum of 2 characcters long and a max of 6 characters.


### Character Classes

Character classes will be any characters a-z, 0-9, and characters such as a .

### Grouping and Capturing

Parenthesis is used for grouping in regex. Grouping is used to seperate characters from literal characters. It also helps to isolate parts of the string.

``/^[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+@[a-zA-Z0-9-]+(?:\.[a-zA-Z0-9-]+)*$/.``

### Bracket Expressions

Bracket expression is used to define what characters will be matched.

``[a-zA-Z0-9-]+`` matches what comes after the '@'

### Greedy and Lazy Match

In the email validation we use the + greedy quantifier. It matches the length of the domain name instead of just a small protion of it which the lazy match.

## Author

Github repo: https://github.com/kji00
