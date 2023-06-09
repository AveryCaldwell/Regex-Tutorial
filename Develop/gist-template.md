# 🧠 Explain Like I'm Five: Regex Tutorial 📌

This Regex tutorial explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does. When included in code or search algorithms, regex can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input.

<br>

## Summary 📃
<br>
<!-- Briefly summarize the regex you will be describing and what you will explain.  -->

This tutorial will break down the complexities of regex into simpler terms, hence, "Explain Like I'm Five." The Hex Code is a color code based on the Hexadecimal system. The word hexadecimal is composed of the terms Hexa and Decem. Hex color codes are code values that represent the color values from 0 to 255. The hexadecimal color definition is usually in the six-digit form, i.e., as a sequence of three hexadecimal numbers, each written with two digits, according to the scheme: #RRGGBB. 

    Matching a Hex Value: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

<br>
<hr>
<br>

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)

<br>
<hr>
<br>

## Regex Components

<br>

### Anchors

`/^` #?([a-f0-9]{6}|[a-f0-9]{3}) `$/`


The ` /^ ` anchor signifies a string that begins with the characters that follow it. The `/$` anchor signifies a string that ends with the characters that precede it. Just as with the `^` character, it can be preceded by an exact string or a range of possible matches.

<br>
<hr>

### Quantifiers

/^#`?`([a-f0-9]`{6}`|[a-f0-9]`{3}`)$/

Next, we tackle quantifiers. Quantifiers set the limits of the string that your regex matches. They frequently include the minimum and maximum number of characters that your regex is looking for. Quantifiers are inherently greedy, meaning they match as many occurrences of particular patterns as possible

 The question mark (`?`) tells the parser that the preceding character is optional, but to be "greedy" and capture it if it's there. The length of the hexadecimal color code should be either `6` or `3`, excluding ‘#’ symbol.

<br>
<hr>

### Grouping Constructs

/^#?`([a-f0-9]{6}`|`[a-f0-9]{3})`$/

Grouping constructs have two primary categories: capturing and non-capturing. Capturing groups capture the matched character sequences for possible re-use (including a numbered backreference) and non-capturing groups do not. A grouping construct can be made non-capturing by adding the characters `?:` at the beginning of an expression inside the parentheses.

It is important to note that capturing groups capture the matched character sequences for possible re-use (including a numbered backreference) while non-capturing groups do not. 

This expression has one group consisting of `([a-f0-9]{6}|[a-f0-9]{3})` that is seperated by an OR Operator. Please see __The OR Operator__ below for further explanation.

<br>
<hr>

### Bracket Expressions

/^#?`([a-f0-9]{6}|[a-f0-9]{3})`$/

Bracket expressions are anything inside a set of square brackets ( [ ] ) that represent a range of characters that we want to match. In the Hex Code regex, parenthesese are used to define the bracket expressions. Here is a breakdown:

- [a-f]—The string can contain any lowercase letter between a–f. Keep in mind that this looks for lowercase characters only.
- [0-9]—The string can contain any number between 0–9 

<br>
<hr>

### Character Classes

/^#?`([a-f0-9]{6}|[a-f0-9]{3})`$/

A character class in a regex defines a set of characters, any one of which can occur in an input string to fulfill a match.

The bracket expressions above are considered character classes: [a-f0-9] and [a-f0-9] which searches for the same values. `a-f` searches for letters a-f and `0-9` searches for digits 0-9.

<br>
<hr>

### The OR Operator

 /^#?([a-f0-9]{6}`|`[a-f0-9]{3})$/

 There are two expresions seperated by an OR Operator ( `|` ): `[a-f0-9]{6}` and `[a-f0-9]{3}` . This means that our regex will match any of those two expresions. The `|` tells us that we can have 6 characters OR have three characters instead.

<br>
<hr>


## Author

- Avery Caldwell: [GitHub](https://github.com/AveryCaldwell)
    - A current web development student at the University of Washington

