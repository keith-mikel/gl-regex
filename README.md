# Regex code for General Ledger Accounts

This assigment is created in order to help understand what a regex or regexp is, and give an example of one to explain. 

A few things that a regex can be used for are 

-Search and Find: a regex can be used to search for words, phrases, and patterns in strings and text documents

-Validation: a regex can be used to validate inputs against a given criteria such as phone numbers and emails. This is to ensure they are formatted correctly to fit the given constraint of the data

-Text Manipulation: regex can be used to manipulate text in a systematic fashion, such as replacing, extracting, and reformatting text and patterns.

-Pattern Matching: regex can be used to match complex patterns with methods such as wildcard, optional elements and character ranges

-Parsing: regex can be used to parse and structure unstructured text, this can be used for extracting data from things like log files and web pages

## Summary

This explanation will be for regex code

`r'^[A-Za-z0-9.-]+$'`

this regex code is one that I have worked with in my job that is for creating general ledger accounts for an accounting software. This limits the accounts to use alphanumeric characters, periods, and hypens (I have manually added the hypen on occasions when clients use hypens in their legacy accounts that exsisted before adopting the software). This constraint sets it so that the string created for the account only contains these characters

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

- `^` Caret: this symbol is used in this regex to establish where the string/line should begin
-`$` Dollar Sign: this symbol is used to establish where the string/line will end

Together these are used to ensure that the whole string contained within them matches the constraints

### Quantifiers

-`+` Plus Sign: this quantifier specifies that the at least one of these set of characters `[A-Za-z0-9.-]+` must be used at least once

### Grouping Constructs
There is no use of grouping constructs (parentheses) in this particular regex.

### Bracket Expressions

-`A-Za-z` This grouping specifies that all letters upper and lowercase (english letters) can be used

-`0-9` This grouping specifies that all numeric digits can be used

-`.-` This grouping specifies that periods and hyphens can be used

### Character Classes

-`[A-Za-z0-9.-]`: this sets the whole class of characters that can be matched for any single given character

### The OR Operator

There is no use of the OR operator `|` in this particular regex

### Flags

the `r` at the start of this expression `r'^[A-Za-z0-9.-]+$'` states that this string expression is a raw python string, this prevents backslashes in the string from being treated as escape characters

### Character Escapes

There are no uses of character escapes `\` in this regex 

## Author

For additonal information please check out my github keith-mikel

https://github.com/keith-mikel

or reach me by email at mikel061@umn.edu