# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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

An Anchor is a Regex Component that is used to specify the postion in the string that should be matched. A carot ^ is an anchor at the begining ^efg whould match anything with that starts with efg. A Dollar Sign at the end of efg $ would match anything that ends with efg. 

### Quantifiers
    * Asterisk: Matches 0 or more occurrences of the preceding element. For example, ab*c would match "ac," "abc," "abbc," and so on.
    + (Plus): Matches 1 or more occurrences of the preceding element. For instance, ab+c would match "abc," "abbc," and so on, but not "ac."
    ? (Question Mark): Matches 0 or 1 occurrence of the preceding element. For example, ab?c would match "ac" and "abc," but not "abbc."
    {n}: Matches exactly n occurrences of the preceding element. For instance, a{3} would match "aaa."
    {n,}: Matches n or more occurrences of the preceding element. For example, a{2,} would match "aa," "aaa," and so on.
    {n,m}: Matches between n and m occurrences of the preceding element. For instance, a{2,4} would match "aa," "aaa," and "aaaa."
### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries
There is also the more advanced Word Boundary. `\bword\b` matches the whole word "word" itself. There is also the start or end of a word `\bword` will match "word" only at the begining of a word. `word\b` will match "word" at the end of a word. Also Excluding Word `\Bword\` which matches the "word" itself and not 
### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
