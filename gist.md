# Regex Matching an Email

This gist.md file provides an explanation of the regular expression (regex) /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/, which is used to match an email address.

## Summary

The regex /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ is designed to validate and match email addresses. This regex ensures that the email address consists of a username, followed by the @ symbol, then the domain name, and finally, the top-level domain (TLD). In the subsequent sections, we will explain each component of this regex.

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

The regex begins with the caret ^ and ends with the dollar sign $. These are called anchors and ensure that the regex matches the entire string. In this case, the email address should be the complete string.

### Quantifiers

The + and {2,6} are quantifiers used in this regex.

- The + quantifier means that the preceding pattern should occur one or more times. For example, ([a-z0-9_\.-]+) matches one or more lowercase letters, numbers, underscores, dots, or hyphens for the username.
- The {2,6} quantifier specifies a range of repetitions. In this regex, it is used to restrict the TLD to be between 2 and 6 characters long. For example, ([a-z\.]{2,6}) matches a sequence of lowercase letters or dots with a length between 2 and 6.

### Grouping Constructs

The regex utilizes parentheses () to create capturing groups.

- ([a-z0-9_\.-]+) captures the username part of the email address.
- ([\da-z\.-]+) captures the domain name part of the email address.

### Bracket Expressions

Bracket expressions, enclosed in square brackets [], specify character ranges or sets.

- [a-z0-9_\.-] represents a character range that includes lowercase letters, numbers, underscores, dots, and hyphens. This is used to match characters in the username.
- [\da-z\.-] matches either a digit, lowercase letter, dot, or hyphen. This is used to match characters in the domain name.

### Character Classes

The \d character class matches any digit. In this regex, [\da-z\.-] includes the digit class as part of the domain name.

### The OR Operator

The pipe | character is not used in this regex.

### Flags

Flags are not used in this regex.

### Character Escapes

Character escapes are not used in this regex.

## Author

After 9 years in banking, I finally transitioned to the world of web development & coding. Check me out at my [GitHub](https://github.com/jmcdlungren).
