# Regex Tutorial

```md
GIVEN a regex tutorial
WHEN I open the tutorial
THEN I see a descriptive title and introductory paragraph explaining the purpose of the tutorial, a summary describing the regex featured in the tutorial, a table of contents linking to 
different sections that break down each component of the regex and explain what it does, and a section about the author with a link to the author’s GitHub profile
WHEN I click on the links in the table of contents
THEN I am taken to the corresponding sections of the tutorial
WHEN I read through each section of the tutorial
THEN I find a detailed explanation of what a specific component of the regex does
WHEN I reach the end of the tutorial
THEN I find a section about the author and a link to the author’s GitHub profile
```

## Summary
 The regular expression We will be disecting and looking further into is the expression look at matching an email:

 ```md
 `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
 ```

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Author](#author)

## Regex Components

### Anchors
```md
There are two anchors on regular expressions. Here we cane see that the beginning anchor for this regex is `^`. The characters that follow this anchor should be the first search criteria the system will look for. Thedning anchor in this expression is `$`. The expression will not look for anything pas this point in the expression.
```
### Quantifiers
```md
Quantifiers can be used in a few different ways and within our matching an email regex we can see several different ways of this being used.

The first quantifier is the `+` symbol. This shows that there should be pattern that matches one or more times foolowing it. In this expression we see `+)@(`, indicating the next criteria we are looking for is the `@` symbol in our search.

We also see a quantifier toward the end of our expression. `{2,6}` indicated that after the `.` before it we should see a string that is minimum of 2 variables and maximum of 6.
```
### Grouping Constructs
```md
Grouping constructs are another way of breaking down the sections of an expression. Here we see ```([a-z0-9\.-]+)```. This shows the first section of our expression. We are searching for any criteria a-z and 0-9 and symbols `\ . -`. We end the section with the `+` symbol to show we are finished here and after this sybol is the next thing we should look for.
```
### Bracket Expressions
```md
Bracket expressions are a way of putting search criteria into one statement so the system can look for all variables within that bracket expression. Any search criteria within these `[]`, will be considered as one search criteria for the system. In our matching an email expression we can see the utilization of three bracket expressions.
```
### Character Classes
```md
Character classes are used to make it easier to look for a set of characters. In the matching email regex the use of `\d` is used to search for any digit.
```
## Author
```md
You can find more from me using this link to my GitHub account [GitHub link](https://github.com/jalontuttle)
```
