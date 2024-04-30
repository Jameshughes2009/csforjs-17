# Computer Science for JavaScript Challenge: Regex Tutorial 

Hello this is a comprehensive tutorial on matching email regex using JS

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
Character Classes are short regex expression that apply to a spefifc set of chartacter
- The Email Function in regex uses two `\d` and `..` 
- Character Sets are general defined with in square brackets `[]`
 - `a-z` match charters with the range and is case senstive 
 - `0-9` match number in a ranger between 0 and 9
 - `./` is an escape chacter
 - `\.` Exscaped Character 


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
Grouping Contrsucts in regex are used to group one or more chacter/sub-expressions, They are the variables between found between the parentheses `()` 

In the Email Function that are three different groups 

- Local-Part which matches the username and email address

 - `([a-z0-9_\.-]+)`
- Domian
 - `([\da-z\.-]+)`
- Top-Level Domain
 - `([a-z\.]{2,6})`

### Bracket Expressions
They are used to define a set of characters that can be matched within a single position in a text string. They are denoted by square brackets [...], and any character enclosed within these brackets will become a part of the allowed set.

Part 1 `[a-z0-9_\.-]`
- `a-z`: Matches lowercase letter from `a` to `z`.
- `0-9`: Matches digit from `0` to `9`.
- `_`: Matches underscore character.
- `\.`: Matches literal period (dot) character. The backslash is used to escape the dot since it has a special meaning in regex.
- `-`: Matces the hyphen character.

Part 2 `[\da-z\.-]`
- `\d` another way to say `0-9`
- `a-z`: Matches lowercase letter from `a` to `z`.

Part 3 `[a-z\.]{2,6}`
- `{2,6}` specifices the number of times that prevous function must be matched


## Author

Find My GitHub Link at [James Hughes](https://github.com/Jameshughes2009)

GitHub-Gist: [Link](https://gist.github.com/Jameshughes2009/fc705be9849138dec47fc272a70ef3aa)

Git Hub Repo: [Link](https://github.com/Jameshughes2009/csforjs-17)
