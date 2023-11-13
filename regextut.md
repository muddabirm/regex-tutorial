#  REGEX tutorial
regular expressions are defined as search patterns used for matching, manipulating, or searching for text. these can be used to find certain characters or match them in a certain way specific to your search query. You can do more than just literally search for something 

## Summary


This is the example regex I will be using to demonstrate all the parts of a regex expression.\
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/\
This regex is a hexadecimal value. Each character in this code snippet provides the search with many ways to filter out certain characters when looking for the matching string.
A hexadecimal is commonly used in CSS for RGB colors. 


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
Anchors are what define where a certain character begins or ends in a string.
for example ^ anchor means that the character after it must match exactly and the $ means the preceding character must match exactly.
So in our case, the string starts matching characters from the start till the end because the anchors are located at the start and the end of the expression.
### Quantifiers
these are used to limit the amount of characters overall in the string. In this case {6} and {3} in the string tell the search to match 6 characters or 3 characters respectively. 
### OR Operator
this character is used to say that the string doesn't need to have all these in the same order it breaks the pattern.
in this case the or operater is the | character which groups  [a-f0-9]|[a-f0-9] the string as shown.
### Character Classes
this class is used to match different types of characters in an expression. These are the characters as shown:
. = matches new line characters
\d = matches numeral digits
\w = matches alphanumeric characters
\s = matches whitespaces like line breaks or indents from tab

### Flags
define the characteristics of a search if it is global "g", case sensitive "i" or a multi-line search "m"


### Grouping and Capturing
 these characters are used to tell the search if a sequence of characters can be re-used
 if "?" is in the parameters it means it is non-capturing and does not re-use the sequence of characters like in our search.
### Bracket Expressions
bracket expressions are useful for giving you a range on what characters in a string can be used like for example in our search everything in the first set of brackets [a-f0-9] can be used as a result and respectively everything in the second set of brackets as well [a-f0-9]. lowercase a-f and numbers zero to nine.
### Greedy and Lazy Match
greedy characters match as many characters as possible in a search and lazy characters match as little as possible in a search. * and + are greedy, but ? and *? are considered lazy.
### Boundaries
boundries specifically define a location in a search where characters should match for example a ^ which means the beginning of a string should match exactly.
or alternatively, a $ which means the character before it should match exactly these are also known as anchors
### Back-references
back-references are \ characters they are used to refer to the previous search or group of searches
### Look-ahead and Look-behind
look behind and look ahead characters tell you to look for a search pattern that is behind a certain character or ahead of a certain character
(?<=) = means look behind
(?=) = means look ahead
## Author

created by muddabir masood a full-stack web developer: https://github.com/muddabirm