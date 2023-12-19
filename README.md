# Email Validation Using Regular Expressions (regex) Tutorial

This gist covers what a regular expression or regex is and how it can be used in coding for validation, matching, searching, extracting, and manipulating various text patterns. Regular expressions can seem very confusing, This tutorial will simplify the regular expression for validating an email address.

## Summary

The Following Regular Expression for the tutorial is used for matching and validation of a email address
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`<br>
This regular expression is broken down into 3 categories, the first part of this regex is an email username and the `@` symbol followed by domain name finished with a dot and top-level domain name. This regex would match a generic email address, for example `abc@gmail.com`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components
This regex `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` has many different components that make sure it can verify an email address. The `^` and `$` are called anchors that represent the start and end of the string, when used together that match the entire string. The parenthesis `()` are the capturing groups that are used to capture and extract specific matched text and apply modifications to specific parts of the pattern. The brackets `[ ]` are bracketed expressions that define valid characters to match a single character at its position in the string. There are also escaped characters `\.` which treat the `.` like a literal character so it matches a literal dot like in .com. The {} part of the last section is quantifier used to set top level domains like .com to be between 2 and 6 characters.


### Anchors
This regex expression uses two anchors. the first is the Caret `^`: The caret anchor matches the starting position of a line or string of characters used to anchor the beginning of a regex pattern. In this code the caret is used outside the square brackets to match the start of the email username `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` 
This regex expression also uses the Dollar Sign `$`: The dollar sign anchor matches the end of the string or a line if it's used with a multiline flag. In this code the dollar sign and caret together are used to match the entire string `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

### Quantifiers
This regex expression uses The Quantifier plus `+` sign which is used directly outside the bracket to match the previous characters inside the brackets one or more times for both the user name in group 1 `([a-z0-9_\.-+])` and the domain name in capturing group 2 `([\da-z\.-]+)` The part of the expression `{2,6}` before the `$` anchor is a numeric quantifier which is used for the top level domain name between an minimum of two and maximum of 6, an example of a domain name is .com or .gov

### Character Classes
Character classes use brackets [] which are more complex than bracket expressions that define a set of characters to match a single character against. The character classes of the regex expression are broken down into 3 sections, the email username, the domain name, and the top layer domain name. 
The username of the email address section of the email or `([a-z0-9_\.-]+)` `[a-z]` matches any lowercase character from a to z, `[0-9]` matches any digit from 0 to 9, `[\_.-]` matches underscores, dots and hyphens characters. This allows for the email username to use lowercase letter, digits, underscores, dots, and hyphens in the username. 
The character class for the domain part of the email address starts after the @ symbol like @aol or @gmail, it is found in this section `([\da-z\.-]+)`. `[\d]` matches any digit 0 to 9, `[a-z]` matches any lowercase letter from a to z \.- matches dots and hyphens. This character class allows the email domain name to use digits, lowercase letters, dots, and hyphens.  
The character class for the top layer domain like .com or .edu `([a-z\.]{2,6})`, `[a-z\.]` matches lowercase letter or dots `{2,6}` sets the range to 2-6 characters

### Grouping and Capturing
Grouping uses parenthesis () to group different parts of the regex and treat the like one separate group. Capturing is used to capture and store the matched text inside a group, this regex expression is broken down into 3 different Capturing groups the email username, domain name and top layer domain name. 

The first capturing group comes after the caret anchor the code `([a-z0-9_\.-])` it is used to capture to email user name and allows numbers, lowercase letters and the special characters.

The second capturing group is `([\da-z\.-])` it comes after the at @ symbol and is used to capture the domain part of the email address like Gmail or AOL. It matches one or more of digits, lowercase letters, dots or hyphens. 

The Third capturing group is `([a-z\.]{2,6})` it captures the top level domains like .com or .edu it matches lowercase letters, dots and i needs to be a minimum a 2 and maximum of 6 characters.

### Bracket Expressions
Bracket Expressions are used to define a character class using square brackets []. Bracket Expressions are all a form of Character classes although not all character classes are bracket expressions. Bracket Expressions are basically used like a container that holds multiple options. This regex has 3 Bracket Expressions `[a-z0-9_\.-]` , `[\da-z\.-]` and `[a-z\.]`

### Greedy and Lazy Match
Greedy and lazy matches are an example of a quantifiers, greedy match is default the lazy match uses `?`. In this Regex example `{2,6}` matches the previous tokens between two and six times as many times as needed making it a greedy match.

## Author
This Tutorial was written by Jeff Schori
This is my contact information if there are any questions
- GitHub User Name [GitHub](https://github.com/schorij23) 
- Email address schorij23@gmail.com
