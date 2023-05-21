# Regex Tutorial

This tutorial covers regex as it relates to matching HTML tags for web applications. 

## Summary

Regex, or regular expressions, are commonly used for HTML tag validation. This technique can be used for matching patterns and extracting HTML tags. Certain applications parse HTML content, which this enables them to do. Regular expressions use a number of different nomenclature and rules such as containing the @ symbol, which we will cover further.

Here is an example of code that is within a regular expression for HTML tag validation: 
`<([a-zA-Z][a-zA-Z0-9]*)\b[^>]*>(.*?)<\/\1>`

The following contents will contain the explanation of each piece of the code. 

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
Anchors are also known as tags or elements. These can be used to define the structure and content of web pages. Common examples of HTML tags include the following: 

- '^' (caret): This matches the start of a line or string
- '$' (dollar sign): this matches the end of a line or string
- '\b' (word boundary): this matches a word boundary, allowing you to match whole wordds

### Quantifiers
Quantifiers specify the number of occurrences of a character or a group of of characters. Quantifiers are used for validation purposes. Common quantifiers include the following:
- '*' (asterisk): Matches zero or more occurrences of the proceeding character
- '+' (plus): Matches one or more occcurences of the preceding character or group
- '?' (question mark): Matches zero or one occurrence of the preceding character or group

### OR Operator
The OR operator is used to match vaious versions of the same tag and enables you to specify multiple alternatives for a pattern. Here are several examples of OR operators:
- Matching opening and closing tags of <h1>, <h2>, or <h3>: <h[1-3]>|<\/h[1-3]>
- Matching tags with different attributes: <a\s+href=".+">|<\/a>


### Character Classes
Character classes are used to match specific character ranges in HTML tags. They allow you to define a set of charactters that can match specific positions in a pattern. Here are several examples: 
- matching alphanumeric characters:
    - Character class: [A-Za-z0-9]
- matching any digit:
    - Character class: [0-9]

### Flags
In regular expressions, character flags are used to modify the behavior of the regex pattern matching.
- 'i' ignores case
- 'u' unicode
- 's' Dot (.) will match characters including newline

### Grouping and Capturing
Grouping and character classes are useed to group multiple expressions togetther and define a set of characters to match, respectively. 

Grouping involvs the following:
- Parentheses are used for grouping characters or expressions together.

Character Classes:
- Square brackets are used to define a character class

### Bracket Expressions
These are also known as character classes and are used to define a set of characters to match. Here are some examples of bracket expressions for HTML
- Negation: matches any non-digit character

### Greedy and Lazy Match
- 'Greedy' involves matching the longest possible string. Greedy behavior involves the Greedy quantifier telling the engine to match instances of the subpattern
- 'Lazy' matching is done with the shortest possible string. This is done by appending a question mark to the end of a regular quantifier. This tells the engine to match as few of the quantified tokens as needed

### Boundaries
Boundaries are defined in regex with the '\b' character. These boundaries are usd to define specific positions in the input text when a match should occur. They're not actual characters; instead they are assertions about the position of characters.
Common boundary assertions in regex include the following:
1. Word Boundary ('\b'):
- This matches the wordd in hello world
2. Start of Ling ('^):
- Pattern matches the pattern only if it appears at the beginning of a line

### Back-references
Back references are used to refer to previously matched group within the patter. They are denoted with the '\' symbol followed by a number representing the group number. There are several examplees of how back references can be used:
1. Matching Repeated Words
- Regex `(\b\w+\b)\s+\1`
- This captures a wordd using the '\b\w+\b' pattern and then uses the bak referencce to mattch the same word again
2. Matching HTML Tags
- Regex `<(\w+)>.*<\/\1>`
- This uses HTML tags to ensure the opening and closing tags math. It captures the tag name using (\w+) and uses the back references to match the corresponding closing tags

### Look-ahead and Look-behind
Lookahead and lookbehind are zero-width assertions that allow you to create conditions for matching patterns in final results. This enables pattern specification that are uttilized for various conditions.

## Author

Nabeel Khan is a current senior product manager at Amazon and a student of the Georgia Tech EdX Bootcamp. The links below send to the rest of this repository and his overall GitHub profile.

Repository: 
https://github.com/nabeekha/Regex-tutorial 

Link to Github Profile:
https://github.com/nabeekha 

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
