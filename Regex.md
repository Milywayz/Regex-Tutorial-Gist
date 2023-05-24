# Regex Tutorial Gist

This gist will be all about better understanding what a Regex is and the purpose of a Regex. I will talk about a specific Regex that I will find useful to know about for future use and hopefully you as well.

## Summary

I will be explaining a "Matching an Email" Regex, which will include a better understanding of each component of the Regex and what use you can have with it.
A matching an Email Regex code looks like this: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Sited Sites](#sited-sites)

## Regex Components

### Anchors

An Anchor is not matching any characters together but inserting the characters into the Regex for it to become a string or for matching. 
The Anchors for the email are ^ which is for starting the regex string. And the $ which ends the regex string of the email to match.

### Quantifiers

There are two quantifiers in the email regex code and they are the + and {2, 6}. The + is for matching the the code to the left of the symbol.
So [a-z0-9_\.-]+ the + is making sure that it matches what's inside the square brackets [].
The {2, 6} is that [a-z\.] can only between 2-6 characters long for that last part of the code line.

### Grouping Constructs

There are three different groups that are in this email regex. The first group is ([a-z0-9_\.-]+) which is for the users name. Then it's followed by the @
symbol which is where group two comes in ([\da-z\.-]+) for what domain they are using. The final group is ([a-z\.]{2,6}) and thats for top level domains
like .com or .org.

### Bracket Expressions

Just like how there are three groups in the email regex, there are three bracket expressions too. They are expressions that are telling us to match what rules are given withing the brackets. 
[a-z0-9_\.-] is matching lowercase alphabet letters a-z, numbers that are between 0-9, _ (underscores), . (periods), and - (hyphens).
([\da-z\.-]+) is for matching that can use multiple digits or one, alphabet letters a-z, . (periods), and - (hyphens).
[a-z\.] is matching for alphabet letters a-z.

### Character Classes

There is only one character class inside the email regex and it's /d inside ([\da-z\.-]+). /d matches one digit only that's in the domain.

### Sited Sites

I used two different websites for helping me learn more about the email regex and will link them down below:
https://www.rexegg.com/regex-anchors.html
https://www.keycdn.com/support/regex-cheat-sheet

## Author

Thanks for reading, you can find my profile here if you want to see more: https://github.com/Milywayz

