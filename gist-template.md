# Regex (Regular Expressions)

regex allows the user to match paterns of a string. a regex is a sequence of characters that defines a search patern for text.
regex can be used in any programing language (javascript, python, c#, etc.). unlike standard lines of code however, regex are writen in an almost
cryptic like way. an example of a regex would be "\(?\d{3}[-.)](\d{3})[-.]\d{4}". this regex is searching for phone numbers that are writen in three different ways (123-456-7890, 123.456.7890, & (123)456-7890). 


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
a regex is always seen as a literal so it needs to begin with the "\" (back slash) character. as shown before, the phone number regex is: 
"\(?\d{3}[-.)](\d{3})[-.]\d{4}"

once it begins, it will execute the following parts which are written in the regex. these are the anchors, quantifires, grouping constructs, and bracket expressions. 

### Anchors
anchors are use to say when a string should start and when it should stop. the phone number expression shown in this demo doesn't use anchors but usually,the characters that would be used for regex are '^' and '$'. the '^' says that the string starts here amd the '$' says that the string stops here. 

### Quantifiers
quantifiers act as inhibitors to regex strings, limiting the amount of caracters that are being searched. in this regex, the '?' quantifier is being used which does the following. 

? - matches the patern zero or one time

### Grouping Constructs
grouping constructs catch and match identical characters and reuse them multiple times. the following example is a grouping construct that 
catches numbers.

\d{3} - matches three digits between 0 and 9
\d{4} - matches four digits between 0 and 9
### Bracket Expressions
bracket expressions are used to identifie specific characters writen inside of "[]"(square brackets). in the following example, we are trying to get
the characters '-', '.', and '()'. which are used in different phonenumbers.

[-.)] - matches characters
### Character Classes
regex are amde up of two components, a meta character and a literal character. a meta character is the primary character that is input in a string. a literal character is any character that comes after the meta character. 

"Regex"

using the word regex as an example, the 'R' in the word is a meta character and 'egex' is made up of literal characters.

### The OR Operator
or operators are another way of writing groug constructs, the only major diference is in how it's written. for example, instead of using '\d{3}' or 
'\d{4}', we can just use the following.

'\d{1|2|3}'
or
'\d{1|2|3|4}'

### Flags
flages are placed in the back of a regex. they add an extra function once the regex is finshed working. this example doesn't use a flag ath the end but here are some examples of flags

g - test all matches in string 
i - cases are ignoreg in match
m - treats string as multiple lines

### Character Escapes
character escapes releace characters that are not being used, if not used then the string would be interupted. for example, in '\d{3}' we are only looking for three numeric characters. once all three are established, all others are released and ignored.


## Author
https://github.com/M1guelPerez01
