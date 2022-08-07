# Regular Expressions:  Matching an Email

Regular expressions to the non-tech person may appears as a jumbled mess of characters or some intricate level of code.  However, once broken down the regex components are very helpful in allowing the ability to search for direct matches of non-standard strings.

## Summary

The regular expression that will be reviewed with be matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
Since a regular expression is considered a literal, the pattern must be wrapped in slash characters (/).  The other parts of teh regular expression will be discussed below in their corresponding section.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Character Escapes](#character-escapes)


### Anchors

The anchors are represented in our email regular expression as the ^ and $.  The ^ anchor is generally found in the beginning of the regex and signifies a string that begins with the characters that will follow it.  The $ anchor is found near the end of the regex and show that the regex will end with the characters that preceed it.

### Quantifiers

Quantifiers set the limits of the string the regex matches.  This will generally include the minimum and maximum number of characters the regex is looking for. In this particular regex of the email, we have {2,6} which will represent that we want to find the preceding string patterns a minimum of 2 times and a maximum of 6 times.

### Grouping Constructs

Grouping constructs are found within the email regex and are represented as the paranthesis ().  This is used to group a section of a regex and each section within the paranthesis is known as a subexpression.  In the email regex we can see that we have 3 separate grouping constructs.

### Bracket Expressions

Bracket Expressions are found with the email regular expression.  These are represented as ([]) square brackets and will represent a range of characters that are being matched.  Within teh square brackets  hyphens can be used between alphanumeric characters to represent a range of those possible characters  For example, [a-z] would signify any lowercase letter between a-z and the same for the 0-9 found within the regex.  In the email regex, lowercase a-z, numbers 0-9, underscores, backslash, periods, and dashes are ranges of characters that we want to match. 

### Character Classes

Within the email regex there is one character class that can be found.  It is (\d), which matches any Arabic numeral digits, or similar to [0-9].

### Character Escapes

Character Escapes are used to help a character escape so the regex looks for the character that follows it.  This is due to certain characters will be used as a quantifier when needing to be searched for instead.  INt he email regex we have (\.) seen a few times.

## Author

Akira Klotzbach is a junior web developer studying with the University of Arizona.  
https://github.com/Raklotzbach

