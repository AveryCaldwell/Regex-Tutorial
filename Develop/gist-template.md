# 🧠 Explain Like I'm Five: Regex Tutorial 📑📌

This Regex tutorial explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does. When included in code or search algorithms, regex can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input.

## Summary 📃

<!-- Briefly summarize the regex you will be describing and what you will explain.  -->

This tutorial will break down the complexities of regex into simpler terms, hence, "Explain Like I'm Five." The Hex Code is a color code based on the Hexadecimal system. The word hexadecimal is composed of the terms Hexa and Decem. Hex color codes are code values that represent the color values from 0 to 255. The hexadecimal color definition is usually in the six-digit form, i.e., as a sequence of three hexadecimal numbers, each written with two digits, according to the scheme: #RRGGBB. 

Matching a Hex Value: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/



## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

<br>
<hr>
<br>

## Regex Components

<br>

### Anchors

`/^` #?([a-f0-9]{6}|[a-f0-9]{3}) `$/`


The ` /^ ` anchor signifies a string that begins with the characters that follow it. The `/$` anchor signifies a string that ends with the characters that precede it. Just as with the `^` character, it can be preceded by an exact string or a range of possible matches.

<br>

### Quantifiers

/^#`?`([a-f0-9]`{6}`|[a-f0-9]`{3}`)$/

Next, we tackle quantifiers. Quantifiers set the limits of the string that your regex matches. They frequently include the minimum and maximum number of characters that your regex is looking for. Quantifiers are inherently greedy, meaning they match as many occurrences of particular patterns as possible

 The question mark (`?`) tells the parser that the preceding character is optional, but to be "greedy" and capture it if it's there. The length of the hexadecimal color code should be either `6` or `3`, excluding ‘#’ symbol.


Next, inside the first group (first group of parentheses), we can have two different situations. The first is any lowercase letter between a and f or a number six times. The | tells us that we can also have three lowercase letters between a and f or numbers instead.

Finally, we want the end of the string ($). We also use the case insensitive flag by adding an i at the end of our expression. This will allow us to match #ffffff as well as #FFFFFF.



<br>

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

- Avery Caldwell: [GitHub](https://github.com/AveryCaldwell)
    - A current web development student at the University of Washington

