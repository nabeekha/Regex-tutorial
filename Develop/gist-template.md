# Regex Tutorial

This tutorial covers regex as it relates to matching HTML tags for web applications. 

## Summary

Regex, or regular expressions, are commonly used for HTML tag validation. This technique can be used for matching patterns and extracting HTML tags. Certain applications parse HTML content, which this enables them to do. Regular expressions use a number of different nomenclature and rules such as containing the @ symbol, which we will cover further.

Here is an example of code that is within a regular expression for HTML tag validation: 
<([a-zA-Z][a-zA-Z0-9]*)\b[^>]*>(.*?)<\/\1>

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
- Matching <a> tags with different attributes: <a\s+href=".+">|<\/a>

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

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
