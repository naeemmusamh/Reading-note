# Regex tutorial — A quick cheatsheet by examples

Regular expressions are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern.

Fields of application range from validation to parsing/replacing strings, passing through translating data to other formats and web scraping.

One of the most interesting features is that once you’ve learned the syntax, you can actually use this tool in (almost) all programming languages.

# Basic topics

1. Anchors — ^ and $

|examples |explanations|
|---------|------------|
|^The |matches any string that starts with The|
|end$|matches a string that ends with end|
|^The end$ |exact string match (starts and ends with The end)|
|roar |matches any string that has the text roar in it|

2. Quantifiers — * + ? and {}

|examples |explanations|
|---------|------------|
|abc*      |matches a string that has ab followed by zero or more c -|
|abc+      |matches a string that has ab followed by one or more c|
|abc?      |matches a string that has ab followed by zero or one c|
|abc{2}    |matches a string that has ab followed by 2 c|
|abc{2,}   |matches a string that has ab followed by 2 or more c|
|abc{2,5}  |matches a string that has ab followed by 2 up to 5 c|
|a(bc)*    |matches a string that has a followed by zero or more copies of the sequence bc|
|a(bc){2,5}|matches a string that has a followed by 2 up to 5 copies of the sequence bc|

3. OR operator — | or []

|examples |explanations|
|---------|------------|
|a(b|c) |matches a string that has a followed by b or c (and captures b or c)|
|a[bc-  |same as previous, but without capturing b or c|

4. Character classes — \d \w \s and .

|examples |explanations|
|---------|------------|
|\d|matches a single character that is a digit|
|\w|matches a word character (alphanumeric character plus underscore|
|\s|matches any character|

Use the . operator carefully since often class or negated character class are faster and more precise.

\d, \w and \s also present their negations with \D, \W and \S respectively.

For example :
\D will perform the inverse match with respect to that obtained with \d.

\D - matches a single non-digit character

In order to be taken literally, you must escape the characters ^.[$()|*+?{\with a backslash \ as they have special meaning.

\$\d  - matches a string that has a $ before one digit

# Flags

We are learning how to construct a regex but forgetting a fundamental concept: flags.

A regex usually comes within this form /abc/, where the search pattern is delimited by two slash characters /. At the end we can specify a flag with these values.


1. g (global) does not return after the first match, restarting the subsequent searches from the end of the previous match


2. m (multi-line) when enabled ^ and $ will match the start and end of a line, instead of the whole string


3. i (insensitive) makes the whole expression case-insensitive (for instance /aBc/i would match AbC)

