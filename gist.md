# Regex: A Beginner's Guide

Regular expressions (regex) are powerful tools to match patterns and process text. In this guide, we'll cover an overview of regex syntax and its components. Hopefully, by the end, you'll have a better understanding of how to build regular expressions.

## Summary

```javascript

    /\bmessy\b/

```

We'll use the above regex example in this guide. This example matches the word "messy" in a text. We will cover the following regex components:

- Anchors
- Quantifiers
- Grouping Constructs
- Bracket Expressions
- Character Classes
- The OR Operator
- Flags
- Character Escapes

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

Anchors are used to match the position of a pattern in the text. The ^ (caret) character matches the beginning of a line, and the $ (dollar sign) character matches the end of a line.

The following displays the word "messy" at the beginning of a line:

```javascript

    /^messy/

```

The following displays the word "messy" at the end of a line.

```javascript

    /messy$/

```

### Quantifiers

Quantifiers detail how many times a pattern should occur. Examples of this are as follows:

- "*" means that the preceding pattern can occur zero or more times. An example of this is:

    This matches as either "messy" or "mey"hnjjjjjjjjjjjjjjjjjjjjjjjjjjjjjjj

    ```javascript

        /mes*y/

    ```

- "+" means that the pattern can occur one or more times. An example of this is:

    This matches as either "messy" or "mesyyy"

    ```javascript

        /mes+y/

    ```
- "?" means that the pattern can occur zero or one time. An example of this is:

    This matches as either "messy" or "mey"

    ```javascript

        /mes?y/

    ```

### Grouping Constructs

Grouping constructs are used to group patterns together. This is done by way of parentheses "()". As an example:

This would match "messy" or "cat".

```javascript

    /(messy|cat)/

```

### Bracket Expressions

Bracket expressions are used to match any one of a set of characters. As an example:

This regex matches any one of the vowels a, e, i, o, or u.

```javascript

    /[aeiou]/

```

### Character Classes

Character classes are used to match any one of a set of characters. They are similar to bracket expressions, but have a different syntax. As an example:

This regex matches any digit.

```javascript

    /\d/

```

### The OR Operator

The OR operator is used to match any one of a set of patterns. The pipe | is used to separate the patterns. As an example:

This would match "messy" or "cat".

```javascript

    /messy|cat/

```

### Flags

Flags are used to modify the behavior of a regex. As an example:

The i flag makes the regex case-insensitive, so it matches "messy", "Messy", and "MESSY".

```javascript

    /messy/i

```

### Character Escapes

Character escapes are used to match special characters. As an example:

This regex matches a period.

```javascript

    /\./

```

## Author

After 9 years in banking, I finally transitioned to the world of web development & coding. Check me out at my [GitHub](https://github.com/jmcdlungren).
