# Python Regular expression 

## .
    A period. Matches any single character except the newline character.

## ^
     A caret. Matches the start of the string.

## $ 
    Matches the end of string.

## [abc] 
    Matches a or b or c.

## [a-zA-Z0-9] 
    Matches any letter from (a to z) or (A to Z) or (0 to 9).

## \ 
    Backslash.
    -   If the character following the backslash is a recognized escape character, then the special meaning of the term is taken (Scenario 1)
    -   Else if the character following the \ is not a recognized escape character, then the \ is treated like any other character and passed through (Scenario 2).
    -   can be used in front of all the metacharacters to remove their special meaning (Scenario 3).

## \w 
    Lowercase 'w'. Matches any single letter, digit, or underscore.

## \s 
    Lowercase 's'. Matches a single whitespace character like: space, newline, tab, return

## \d 
    Lowercase d. Matches decimal digit 0-9.

## \b 
    Lowercase b. Matches only the beginning or end of the word.

## + 
    Checks if the preceding character appears one or more times starting from that position.

## * 
    Checks if the preceding character appears zero or more times starting from that position.

## ? 
    Checks if the preceding character appears exactly zero or one time starting from that position.

## {x} 
    Repeat exactly x number of times.

## ( )	
    Creates a group when performing matches.

## < >	
    Creates a named group when performing matches.