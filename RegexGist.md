# RegEx Gist

Regex is used to define a specific patteren.  This can be used to validate user input to make sure they are entering valid information.

## Summary

In this Gist, I will cover how to verify a email address using RegEx using the following expression:

```
 /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)

## Regex Components

A regex is considered a literal, so the pattern must be wrapped in slash characters (/). If we examine the “Matching a Email Addres” regex, you'll see that this is true:

```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```


### Anchors

The characters ```^``` and ```$``` are the anchors in the statement and mark the start and finish of the express being evaluated.

The ``^`` anchor signifies a string that begins with the characters that follow it. This could be in one of two formats:

An exact string match, such as ```^The```, where the strings "The" or "The person" match, but "the" and "the person" do not. This is because a regex is case-sensitive.

A range of possible matches, displayed using bracket expressions. We'll discuss this in the next section.

The ```$``` anchor signifies a string that ends with the characters that precede it. Just as with the ```^``` character, it can be preceded by an exact string or a range of possible matches.

### Quantifiers

Quantifiers set the limits of the string that your regex matches (or an individual section of the string). They frequently include the minimum and maximum number of characters that your regex is looking for.

```*``` —Matches the pattern zero or more times

```+``` —Matches the pattern one or more times

```?``` —Matches the pattern zero or one time

```{}``` —Curly brackets can provide three different ways to set limits for a match:

```{ n }``` —Matches the pattern exactly n number of times

```{ n, }``` —Matches the pattern at least n number of times

```{ n, x }``` —Matches the pattern from a minimum of n number of times to a maximum of x number of times

Each of these quantifiers can be made lazy by adding the ? symbol after it, meaning it will match as few occurrences as possible.



### Character Classes

### Grouping and Capturing

### Bracket Expressions

## Author

This tutorial is by Shuterspeed1000.  Other projects and information can be found at https://github.com/shutterspeed1000.
