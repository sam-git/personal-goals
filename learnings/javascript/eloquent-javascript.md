
http://eloquentjavascript.net/08_error.html#p_E0PMYRZC2c
---
`debugger` statement in javascript will pause the code and open the browsers debugger at that point of execution.

in non strict mode, `this` is functions that are not called as methods refers to the global scope object. using strict mode makes it hold the value `undefined`. [link](http://eloquentjavascript.net/08_error.html#h_u1jlTq3i42)

http://eloquentjavascript.net/09_regexp.html
---

`<regex>.test(<string>)` is the simplest ay to regex and returns a boolean.

Doing this in a regular expression in the browser breaks it :(
`/([01]+)+b/.test("010101001010010101010101010100101001")`
[link](http://eloquentjavascript.net/09_regexp.html#p_VxCrsg7UEp)

`<regex>.exec(<string>)`
is the same as
`<string>.match(<regex>)`

#### Square Brackets
- . loses its special meaning inside square Brackets
- \- between two indicates a range based on the characters unicode numbers.
- a caret ^ immediately after the opening square bracket inverts the character set so it will match anything *except* the characters in the set. [link](http://eloquentjavascript.net/09_regexp.html#p_HqQEZsitdl)

#### Curly Braces
Indicate a pattern should occur a precise number of times.
eg
- `\d{2}` is 2 numeric characters
- `\d{1,2}` means 1 or 2 numeric characters.
- `\d{,2}` is at most 2
- `\d{2,}` is at least 2
