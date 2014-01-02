#JavaScript Allongé Notes
https://leanpub.com/javascript-allonge

##1 The first sip: Basic Functions
You recall that we have two types of values with respect to identity: Value types and reference types. Value types share the same identity if they have the same contents.Reference types do not.

Which kind are functions? Let’s try it. For reasons of appeasing the JavaScript parser, we’ll enclose our functions in parentheses:

(function () {}) === (function () {})
  //=> false
Like arrays, every time you evaluate an expression to produce a function, you get a new function that is not identical to any other function, even if you use the same expression to generate it. “Function” is a reference type.

(function () {})()
  //=> undefined
What is this undefined?

undefined

In JavaScript, the absence of a value is written undefined, and it means there is no value. It will crop up again. undefined is its own type of value, and it acts like a value type:
