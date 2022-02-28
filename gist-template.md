**Finding A Phone Number**

Within many Databases, user data is important to so many people and one of the most important pieces of DATA that a 'USER' can provide is their phone number.  It helps keep in contact and usually can provide a direct correlation to the specific user.   Phone numbers are usually connected to the 'USER' for a longer period of time and are much harder to change, unlike emails. 
Regualar Expression (RegEx) is a way to search through a string of text in a powerful way.

Summary
I will be explaining the following expression, in order to target and group together different types of provided phone numbers.  Whether they be a local number or international. Regardless of format.


The Expression
/(?:(\+1)[ -])\(?(?<areacode>\d{3})\)?[ -]?(\d{3})[ -]?(\d{4})/gm


Regex Components

Anchors
    
    In this example, the normal anchors (ex: '^' and '$') are not going to be used, because the Regular Expression is meant to search the whole page (globally). Which is shown as '/g'.

Quantifiers
    
    '*','?' and '{}' are used.

   * = Matches any string that contains zero or more occurrences of what follows it.
   ? = Matches any string that contains zero or one occurrences of what follows it.
   {} = Matches any string that contains a sequence of whatever variable is inserted between the brackets, can be more than one variable, which would be seperated by a comma.

OR Operator
    
    '|' and '[]'

Character Classes
    
    Distinguish different types of characters. For example, distinguishing between letters and digits.
    '\d','\w','\s' and '.'

Flags
    
    Regular expressions have optional flags that allow for functionality like global searching and case-insensitive searching. These flags can be used separately or together in any order, and are included as part of the regular expression.
    /g = G standing for globally. Perform a global match, finding all matches rather than stopping after the first match.
    /m = M standing for searching multiple lines. Will perform multiline matching.
    /i = I Perform case-insensitive matching.

Grouping and Capturing

    By placing part of a regular expression inside round brackets or parentheses, you can group that part of the regular expression together. This allows you to apply a quantifier to the entire group or to restrict alternation to part of the regex. Only parentheses can be used for grouping.

Bracket Expressions

    A bracket expression is either a matching list expression or a non-matching list expression. It consists of one or more expressions: ordinary characters, collating symbols, character classes, or range expressions.

Author

    Christian Vasquez is currently Rutgers Bootcamp student. He has spent over 10 years in automotive sales. And is excited to venture into the tech world.
    https://github.com/vasqc/Regex-Tutorial
