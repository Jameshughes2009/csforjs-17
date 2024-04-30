# Computer Science for JavaScript Challenge: Regex Tutorial 

Introductory paragraph (replace this with your text) test

## Summary

For this week's Challenge, we have been assigned to create a technical tutorial that explains how a particular regular expression functions. A regular expression, or regex, is a search pattern used by developers. In the tutorial, you’ll break down each part of the expression and describe what it does.

Is this Tutorial we will be analysing the,

- Matching an Email Regex:  `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
- Definition: Anchors provide a way to limit how a regex matches a particular string by telling the regex engine where matches can begin and where they can end. 
There are two types of Anchors:
 1. Start Anchor `^` for the email expression but some case they can start with `\A`
 2. End Achor are Generally `$` but is the same way as above can aslo be `\Z`

### Quantifiers
In Regex, a “quantifier” specifies how many times a certain character or group of characters should appear in the input string. They allow you to control the number of occurances of a pattern as well. 
 - for this expiression the `+` is Quantifiler and it mean match 1 or more of the preceding token 
 - for `{2,6}`: This group matches a sequence of 2 to 6 lowercase letters or dots. This means that the email address must end with a two to six letter top-level domain, such as .com, .edu, or .co.uk. 
 - From the example we choice `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`:

1. Quantifier `+` : Matches "one or more" occurrences.
   - `([a-z0-9_\.-]+)`: Matches one or more lowercase letters, digits, dots, underscore  or hyphens.
   - `([\da-z\.-]+)`: Matches one or more digits, lowercase letters, dots, or hyphens.

2. Quantifier `{2,6}` : Matches between 2 and 6 occurrences items.
   - `([a-z\.]{2,6})`: Now er will get  a sequence of 2 to 6 lowercase letters or dots.




### OR Operator
The OR operator will allow regex to match with either one pattern or another but cannot be both
- In this example there is no OR Operator that is used
- General Syntax `|`
### Character Classes


### Flags
Flags affect the behavior of regular expressions(regex) by enabling or disabling certain features and are appended to the end of the regex pattern, outside the slashes `/`.
- In Our Regex formual there is no use of flags but there are 6 that may be used going forward
There are six types of flags
 - `i`(ingnore casing): Makes the expression search case-insensitivty.
 - `g`(Global):Makes the expression search for all occurrences.
 - `s`(Dot All): Makes the wild character `.` match newlines as well.
 - `m`(Multiline):Makes the boundary characters `^` and `$` match the beginning and ending of every single line instead of the beginning and ending of the whole string.
 - `y`(Sticky):Makes the expression start its searching from the index indicated in its `lastIndex` property.
 - `u` Unicode: Makes the expression assume individual characters as code points, not code units, and thus match 32-bit characters as well.

### Grouping and Capturing
Grouping Contrsucts in regex are used to group one or more chacter/sub-expressions, They are the variables between `

### Bracket Expressions


### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

Find My GitHub Link at [James Hughes](https://github.com/Jameshughes2009)

GitHub-Gist: [Link](https://gist.github.com/Jameshughes2009/fc705be9849138dec47fc272a70ef3aa)

Git Hub Repo: [Link](https://github.com/Jameshughes2009/csforjs-17)
