# Matching an Email with REGEX –
## /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Summary
A breakdown of the REGEX for matching an email.
Regular Expressions or REGEX are used for authentifications and matching of strings.
 /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ 
 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Author](#author)


## Regex Components
Regex has a wide variety of uses but for now lets start with email matching.

### Anchors
`^` : begins the start of a string

`$` : ends of the string

These characters are at opposite ends, whatever is nested between them is whats being searched through to find an exact match according to the nested characters.

### Quantifiers

`+` : matches the previous token between one and any amount times, as many times as possible, giving back as needed.

`{2,6}`  : matches the previous token between 2 and 6 times. it is used in the last group for the top level domain like .com or .org. for example. .peppermill would be long for the quatifiers and will fail.

### Character Classes
`\d` : matches a single digit character.

### Grouping and Capturing
`()` : whatever characters are capture within these, determines their value. 

There are three sets of open and close parenthesis in this expression.
In the first two sets, the plus quantifier is being used. 
The third set uses `{2,6}` and is quantifying the square brackets.

### Bracket Expressions
`[]` : matches a string if there are any of the specified characters.

`[\da-z\.-]` :
  - any `\d` digit will be matched.
  - any `a-z` character will be matched.
  - any `\.` will be matched.
  - any `-` will be matched.

## Author
Macy Mannix student with UC Davis: Full Stack Coding Bootcamp
Github: https://github.com/macykcool