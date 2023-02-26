# Title (replace with your title)

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

### Anchors
There are two types of anchors, the caret (^) symbol and the dollar sign symbol ($). The caret symbol is used to locate a certain pattern only if it appears at the beginning of a string. While the dollar sign is used to locate a pattern at the end of a string. 


### Quantifiers
Quantifiers is a metacharacter that tells you how many times a character, group, or class appears in a pattern. An asterisk * matches zero or more occureence of a character or group. A plus sign + tells one or more occurrences of a group or character. A question mark ?, will match zero or one occurence of a preceding character or group.
Curly brackets {} will match exactly how many occurences you put inside the curly brackets. Curly brackets {,} with a comma inside will match the number you put inside and more, an example would be {5,}, this would show you 5 or more occurences. Curly brackets with a comma and two numbers inside, as such {2,3} will give you the occurences of the character or group between these two numbers. 

### Grouping Constructs
Grouping constructs can group together regular expression tokens and treath them as one. With grouping constructs you can apply a qunatifier to the entire group, apply alternation to the group, or capture the matches text within the group. 
A capturing group, which works by placing a group of tokens inside a set of parentheses (), can save the matched text into a numbered capture group that you can reference later in the regex or in the replacement text of a search and replace operation. 
The second type of group contruct is a non-capturing group. It is written by placing the group of tokens inside a set of parentheses followed by a question mark and colon. (?:). This contruct does not create a numbered capture group and is useful if you want to group together a set of tokens without capturing the matched text. 
### Bracket Expressions
Bracker expressions are used to specify a set of characters that can match a single character in an input text. It is defined by writting two square brackets, []. If you hyphen between two characters you can include character ranges such as [a-z] or [1-9]. Additionly you can include a caret at the beginning such as [^a-c], which will match any character not within the range of a-c, such as a, b, or c. 
### Character Classes
A character class is used to match any single character from a specific set of characters. You can define a character class by wrapping it i na set of square brackets, []. What ever set of characters inside the brackets is what will be matched with. Predefined sets up common characters are also used, such as \d which matches any digit character, \w which matched with any alphanumberic character, and \s which matches any white spaces such as tabs or space. 
### The OR Operator
THe OR operator is reprented by the pipe symbol "|", and it helps match one or several alternative patterns. It is a way of saying can you match one thing or another, such as white|black, this will match a string with either white or black in it. 
### Flags
Flags are additional parameters that can help modify the behavior of regular expressions. They are added at the end of regular expressions. 
- "i"- ignore case, matches patterns without regard to case sensitivity. 
-"g": global, matches all occurances of a pattern, not just the first one. 
-"m": multiline, changes the behavior of "^" and "$" to match the beginnig and end of each line, rather than the beginning and end of the entire string. 
-"s": dotall, allows the "." metacharacter to match any character, including newlines. 
-"x": verbose, allows you to write regular expressions that are more readable by ignoring whitespace and comments. 
### Character Escapes
Character escape will restore the original literal meaning of the following character instead of the special meaning in regex. To use this you simply need to add a forward slash followed by the character such as \+ or \*. this are important as we might need to write an expression without converting the meaning of a character to something we dont need. 
## Author

A former social worker turned MERN stack developer. A link to my github: https://github.com/cameliabenavides10