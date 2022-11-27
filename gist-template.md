# Regex Tutorial (Phone Numbers)

The purpose of this turorial is to teach new webdevelopers the purpose using a regex. This tutorial will provide insight on what a regex is and how it can be used within your code to identify specific patterns or make sure the input from a user meets certain criteria. I hope you find this useful and are able to implement the lessons into your own code!

## Summary

A regex, also known as a regular expression, is a sequence of special characters used to help define a search pattern within a body of text. This tutorial will focus on a regex to help identify a phone number. The regex focuses on three main sections, the first consitsting of three digits, followed by another section consisting of three digits ending with a third section consosting of four digits. this digit will also allow for an optional section at the beginning that consits of a "+" and or one to two digits. A digit being any number between 0-9.

Below is the regex for identifying a phone number:
```
/^[\+]?[0-9]?[(]?[0-9]{3}[)]?[-\s\.]?[0-9]{3}[-\s\.]?[0-9]{4}$/
```


## Table of Contents

- [Anchors](#anchors)
- [Character Classes](#character-classes)
- [Bracket Expressions](#bracket-expressions)
- [Quantifiers](#quantifiers)

   
## Regex Components


### Anchors

```/^```[\+]?[0-9]?[(]?[0-9]{3}[)]?[-\s\.]?[0-9]{3}[-\s\.]?[0-9]{4}```$/```

```Anchors``` signify the beginning and ending of a regex. This regex is wrapped by the caret (```^```) and dollar sign (```$```). The ```^``` signals the beginning and the ```$``` signals the end of the regex.
    
The entire expression also starts and ends with a slash (```/```) so that the expression is not read literally.

### Character Classes 

```Character Classes``` classify the cxharacters to expect in the regex. While ```0-9```(any number between 0 and 9) and ```a-z```(any letter between A and z) may be some what self explanetory, others are a little more vague. For example, ```\d``` is basically the same as ```0-9```, meaning any digit and ```\s``` allows for a space. ```\_``` allows for an underscore, ```\.``` allows for a period and ```\-``` allows for a dash. 


### Bracket Expressions

/^```[\+]```?```[0-9]```?```[(]```?```[0-9]```{3}```[)]```?```[-\s\.]```?```[0-9]```{3}```[-\s\.]```?```[0-9]```{4}$/

 ```Bracket Expressions``` are, as you may have guessed, anything that lie within a pair of square brackets (```[]```). Brackets are used to show potential characters that may be used.

### Quantifiers

 /^[\+]```?```[0-9]```?```[(]```?```[0-9]```{3}```[)]```?```[-\s\.]```?```[0-9]```{3}```[-\s\.]```?```[0-9]```{4}```$/

 ```Quantifiers``` follow ```Bracket Expressions``` to let you know how many of these characters to expect.This regex uses the quantifiers ```?``` and ```{}```.  The ```?``` is used to say there may be zero or one of the previous characters. The ```{}``` will contain a number which will signify the number of characters to expect. Above you see ```[0-9]{3}``` which means it will look for three digits between zero and nine.

## Author

### Ben Hobson

Ben Hobson is a Los Angeles-based full-stack web development student at UCLA Extension 

GitHub: https://github.com/3enhobson
