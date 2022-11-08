# Hines Regex Tutorial
The purpose of this assignment is to breakdown and discuss a chosen regular expression. A regular expression, known as a regex, is a set of characters used to specify a search patter. Regex are useful for a variety of puposes across almost all programming languages. 

### Summary
In this tutorial, we will look at the following regex: \B#(?:[a-fA-F0–9]{6}|[a-fA-F0–9]{3})\b /g

This regex matches any valid hex color inside a text. 

## Table of Contents
[Anchors](#anchors)
[Quantifiers](#quantifiers)
[OR Operator](#or-operator)
[Character Classes](#character-classes)
[Flags](#flags)
[Grouping and Capturing](#grouping-and-capturing)
[Bracket Expressions](#bracket-expressions)
[Greedy and Lazy Match](#greedy-and-lazy-match)
[Boundaries](#boundaries)
[Back-references](#back-references)
[Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components
### Anchors
Anchors are used to assert something about a string or the matching process. They do not align to any characters. 
Because the regex we are looking at in this tutorial does not have a "beginning" or "end" it does not use the ^ to begin or $ to end.

### Quantifiers
Quanitfiers 'quantify' how many of something (character, group, character class) must be in the input for a match to be found. 

? is a greedy quanifier that matches zero or one time. 

### OR Operator
The OR operator | is used to match an option on either side of the operator while capturing both options. 

The OR operator in the middle of the bracket expressions will try to match the option on either side of the OR operator. 

### Character Classes
Character classes are used to tell the regex engine to match only one out of multiple characters.

Character classes are not used in the example regex. 

### Flags
Flags are used to affect what is returned in the search. 

The example regex includes a global modifier which means it does not return after the first match. 

### Grouping and Capturing
Groups is used to group multiple patters. Groups can be captured where multiple instances of a pattern will be displayed in an array. 
The capturing group is: ([a-fA-F0-9]{6}|[a-fA-F0-9]{3})

### Bracket Expressions
The OR operator [] is similar to the OR operator but does not capture the options.
[a-fA-F0-9] and [a-fA-F0-9] 
Each portion in the brackets is looking to match the following: 
a-f - matches a sigle character in the range a-f and is case senstive 
A-F - matches a sigle character in the range A-F and is case senstive 
0-9 - matches a sigle character in the range 0-9
{6} - matches the previous portion in [] 6 times
{3} - matches the previous portion in [] 3 times

### Greedy and Lazy Match
Greedy quatifiers will match the longest possible string while lazy quatifiers will match the shortest possible string. 

? is a greedy quanifier that matches zero or one time. 

### Boundaries
Boundary markers anchor the pattern to the beginning and end of a line.
In this expamle, \B assert position where \b does not match, and \b asserts position at a word boundary

### Back-references
Backreferences indenfiy a previously matched group and looks for the same match again. 

Backreferences are not used in the example regex.

### Look-ahead and Look-behind
Look-ahead and look-behind, which together are called look-around, tell if a match is possible or not.

Loo-arounds are not used in the example regex.

## Author
Alexa Hines is a programming student in Triolgy's coding bootcamp through Butler University.
https://github.com/a-hines 