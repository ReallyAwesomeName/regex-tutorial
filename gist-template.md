# Regex Tutorial

Let's dive into the world of Regular Expressions (Regex). Regular expressions are powerful tools for pattern matching and manipulating text. In this tutorial, we'll cover various components and concepts of regex to help you master this essential skill.

## Summary

As an example, I will use a the following regex pattern:

```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```

This regex will match email address strings.

## Table of Contents

- [Regex Tutorial](#regex-tutorial)
  - [Summary](#summary)
  - [Table of Contents](#table-of-contents)
  - [Regex Components](#regex-components)
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
  - [Author](#author)

## Regex Components

### Anchors

Anchors are used to match positions in the text rather than characters. Commonly used anchors are:

    ^ Matches the start of a line.
    $ Matches the end of a line.

### Quantifiers

Quantifiers control the number of occurrences of a character or a group in a regex pattern. Common quantifiers include:

    * Matches zero or more occurrences of the preceding character/group.
    + Matches one or more occurrences of the preceding character/group.
    ? Matches zero or one occurrence of the preceding character/group.
    {n} Matches exactly 'n' occurrences of the preceding character/group.
    {n, m} Matches between 'n' and 'm' occurrences of the preceding character/group.

### OR Operator

The OR operator (|) allows you to specify alternatives. It matches either the expression before or after the operator. For example, cat|dog matches either "cat" or "dog."

### Character Classes

Character classes help match any one character from a defined set of characters. Some common character classes include:

    \d Matches any digit (equivalent to [0-9]).
    \w Matches any word character (letters, digits, or underscores).
    \s Matches any whitespace character (spaces, tabs, line breaks, etc.).
    . Matches any character except for a newline.

### Flags

Flags modify how a regex pattern is applied. Common flags include:

    g Global flag. Matches all occurrences rather than stopping at the first match.
    i Case-insensitive flag. Ignores the case when matching characters.
    m Multiline flag. Changes the behavior of ^ and $ to match the start/end of each line.

### Grouping and Capturing

Parentheses () are used for grouping parts of a pattern together. They also allow capturing matched substrings for later use.

### Bracket Expressions

Bracket expressions allow you to match any single character within a specified range or set. For example, [aeiou] matches any vowel.

### Greedy and Lazy Match

By default, quantifiers are greedy, meaning they match as much as possible. Adding a ? after a quantifier makes it lazy, matching as little as possible.

### Boundaries

Word boundaries \b are used to match positions between word and non-word characters.

### Back-references

Back-references (\1, \2, etc.) allow you to match the same text that was previously matched by a capturing group.

### Look-ahead and Look-behind

Look-ahead and look-behind assertions allow you to match a pattern only if it is (or isn't) followed by (or preceded by) another pattern without including the other pattern in the match.

With these components and concepts, you can build complex regex patterns to efficiently search, validate, and manipulate text. Practice is key to becoming proficient with regular expressions.

## Author

This is put together by Jason Geoghegan. My GitHub profile can be found here:

[Jason Geoghegan's Github Profile](https://github.com/ReallyAwesomeName)
