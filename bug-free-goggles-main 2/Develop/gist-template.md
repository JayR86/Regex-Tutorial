# Regular Expression (Regex) Tutorial: All about REGEX

Introductory paragraph (replace this with your text)

## Summary

Welcome to the Regex Tutorial! Regular expressions, commonly known as regex, are powerful tools used for pattern matching and manipulation of text data. In this tutorial, we will break down a specific regex expression and explain each part in detail. By the end, you will have a clear understanding of how the regex works and how to use it effectively in your JavaScript code.

## Table of Contents
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors<a name="anchors"></a>
    Anchors are used to match patterns at specific positions within a string. The two most commonly used anchors are:

        `^` - Matches the beginning of a string.
        `$` - Matches the end of a string.

    For example, the regex /^hello/ matches the word "hello" only if it appears at the beginning of a string. Similarly, the regex /world$/ matches "world" only if it appears at the end of a string.

### Quantifiers<a name="quantifiers"></a>
    Quantifiers define the number of occurrences of a pattern that should be matched. They follow the pattern they are quantifying. Some commonly used quantifiers include:

        `*` - Matches zero or more occurrences.
        `+` - Matches one or more occurrences.
        `?` - Matches zero or one occurrence.
        `{n}` - Matches exactly 'n' occurrences.
        `{n,}` - Matches 'n' or more occurrences.
        `{n,m}` - Matches between 'n' and 'm' occurrences.
    For example, the regex /a+/ matches one or more occurrences of the letter 'a'. The regex /ab{2,4}/ matches 'a' followed by 2 to 4 occurrences of the letter 'b'.

### OR Operator<a name="or-operator"></a>
    The OR operator, denoted by the pipe symbol |, allows you to match one pattern or another. It matches the pattern preceding the pipe symbol or the pattern following it. For example, the regex /cat|dog/ matches either "cat" or "dog" within a string.

### Character Classes<a name="character-classes"></a>
    Character classes allow you to match a specific set of characters. They are enclosed within square brackets [ ] and define a range of characters to be matched. Some common examples include:

        [A-Z] - Matches any Uppercase letter from 'a' to 'z'.
        [a-z] - Matches any lowercase letter from 'a' to 'z'.
        [0-9] - Matches any digit from '0' to '9'.
        [A-Za-z] - Matches any letter (case-insensitive).
    For example, the regex /[aeiou]/ matches any vowel in a string.

### Flags<a name="flags"></a>
    Flags are optional modifiers that can be added to the end of a regex pattern. They modify the behavior of the regex matching. Some commonly used flags include:

        i - Case-insensitive matching.
        g - Global matching (find all matches, not just the first one).
        m - Multiline matching.
    For example, the regex /hello/i matches "hello" case-insensitively, allowing it to match "Hello" or "HELLO" as well.

### Grouping and Capturing<a name="grouping-and-capturing"></a>

    Grouping allows you to treat multiple characters as a single unit and apply quantifiers or modifiers to them collectively. Groups are defined using parentheses ( ). Capturing groups are used to extract the matched content. For example:

        (abc) - Matches the characters "abc" as a group.
        (ab)+ - Matches one or more occurrences of the characters "ab" as a group.
    Capturing groups are especially useful when you want to extract specific parts of a matched pattern. You can access the captured content using special variables or methods in JavaScript.

### Bracket Expressions<a name="bracket-expressions"></a>
    Bracket expressions provide a way to specify a set of characters within square brackets [ ]. They match any single character from the specified set. For example, the regex /[abc]/ matches either 'a', 'b', or 'c'.

    You can also use negation within bracket expressions by placing a caret symbol ^ at the beginning. For example, the regex /[^0-9]/ matches any character that is not a digit.
### Greedy and Lazy Match<a name="greedy-and-lazy-match"></a>
    By default, regex matching is greedy, meaning it tries to match as much as possible. However, there are cases where you may want to perform a lazy match, which matches as little as possible.

    The greedy quantifiers *, +, ?, and {} are made lazy by appending a question mark ? after them. For example, the regex /a+?/ matches the minimum possible occurrence of 'a'. It will match only one 'a' instead of matching as many 'a's as possible.

    Lazy matching is useful when you want to match the smallest possible part of a string or when combined with other components like the OR operator.
### Boundaries<a name="boundaries"></a>
    Boundaries are used to match specific positions in a string, rather than matching actual characters. There are three commonly used boundary symbols:

        \b - Matches a word boundary. It matches the position where a word character is not followed or preceded by another word character.
        \B - Matches a non-word boundary. It matches the position where a word character is followed or preceded by another word character.
        ^ and $ - As mentioned earlier, ^ matches the beginning of a string, and $ matches the end of a string. They can also be used as boundaries.
    For example, the regex /\bhello\b/ matches the word "hello" only if it appears as a separate word, not as part of another word.
### Back-references<a name="back-references"></a>
    Back-references allow you to refer to previously captured groups within the same regex pattern. They are denoted by a backslash \ followed by a digit representing the capturing group number. For example, the regex /(ab)c\1/ matches "abcab" because \1 refers back to the first capturing group, which is "ab".

    Back-references are useful when you want to match repeating patterns or ensure that a specific pattern occurs multiple times.
### Look-ahead and Look-behind<a name="look-ahead-and-look-behind"></a>
    Look-ahead and look-behind are special constructs that allow you to match patterns based on what comes before or after them, without including those parts in the actual match. They are denoted by (?=...) for look-ahead and (?<=...) for look-behind.

    For example, the regex /apple(?= pie)/ matches the word "apple" only if it is followed by the word "pie", without including "pie" in the match. Similarly, the regex /(?<=\$)\d+/ matches one or more digits that are preceded by a dollar sign.

    Look-ahead and look-behind assertions are powerful tools for complex pattern matching, as they provide additional conditions for matching without consuming the actual characters.

    Congratulations! You have now learned about the various components of regular expressions. With this knowledge, you can create powerful patterns to search, validate, and manipulate text data in JavaScript.

    Now go ahead and practice using regular expressions in your code to unlock their full potential!
## Author

    This tutorial was written by  [Jairo](https://github.com/JayR86). He is a passionate web developer with expertise in JavaScript and front-end development. If you have any questions or want to connect, you can reach out to them on GitHub.


