# Matching Hexadecimal Values with RegEX

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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

Here is our example code:

```Matching a Hex Value: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/```


### Anchors

Anchors act as the beginning and end of a seach. The symbol "^" repersents the start of the search, while the symbol "$" repersents where the serch will end. The inputed characters between the two anchors are what will be searched for to ensure a match.

### Quantifiers

Quantifiers set a limit for the string to search through. For the code above, our examples are 6 and 3. The 6 will repersent the full 6 digit value of the hexadecimal. Meanwhile the 3 will repersent the RGB(Red, Green, and Blue) values. 

### Grouping Constructs

Grouping Constructs are identified with a "()". While this method has two main objectives (capturing and non-capturing), for the purpose of this tutorial, we will focus on the
capturing aspect. When we look at the code: ([a-f0-9]{6}|[a-f0-9]{3}), we can tell it is capturing values to match for a specific sequence. If there was a "?:" somwhere in the middle of the code, we would identify it as a non-capturing grouping. 

### Bracket Expressions

Bracket Expressions are identified by "[]". They contain a range of charcaters that need to be matched. For the example above, our expressions are: 
[a-f0-9]. This code is looking to match any variation of letters between "a" and "f". The same is said for the numbers "0" and "9". 

### Character Classes

### The OR Operator

The OR Operator can be identified with a "|" symbol. The purpose of this is to tell the string if the first value is not a match, then search for the second value. For the code provided, we can see that [a-f0-9]{6} is looking for a letter value of anythinbg between a-f witha numerical value between of 0-9 for a total of 6 characters. If it cannot match a value with what is provided, then it will search for a value that matches [a-f0-9]{3}. 

### Flags

### Character Escapes

A Character Escape is repersented by a "\". It escapes a character that would otherwise be interperated literally. For example, the open curly bracket ({) is used to begin a quanitifier, but by adding a backslash before the bracket (\{), it means that the regex should look for the open curly bracket charcater instead of the beginning to define a quantifier.

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
