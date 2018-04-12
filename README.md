# The Jay-esque Style

### *this is javascript*

## Fantastical bits
* Dont add `;` at the end
* If your statement is impure; mark it with a `;` in the front!
* Use arrow functions, and only arrow functions!
* If your function is impure; make it `{{}}`!
    * e.g. No `x => console .log (x)`. It's impure, so `x => {{ ; console .log (x) }}`
* No function statements
* Make your functions generic. Use `x`, `y`, `z`, `w`, `a`, `b`, `c`, ..., for the parameters (Unless they are really specific, obviously unreusable)
* Add spaces between tokens
* Avoid suffixes smaller than the prefix. It is undiscoverable.
    * e.g. This is bad. The significant call operator `()` is undiscoverable! Is this a function or the value?
```
var result = (x => {
   ...
   var computation = step_1 + step_2
   return result
}) ()
```
* Mark your sentence with the one significant prefix (if its in a phrase), hide the rest on the previous line. Encourage the leading member to follow the `[` or `(`
    * e.g. (the prefix here is `o`)
```
var result = Oo (something,
  o (x => x .parent),
  o (R .reduce ((sum, x) => sum + x, 0)))
```
or
```
var q = [ document .querySelector ('fire')
  , document .querySelector ('earth')
  , document .querySelector ('air')
  , document .querySelector ('water') ]
```
* Collapse the `)`s, `}`s, etc.

## Aesthetic bits
* Use tabs
* Use single quotes `''`
* Use snake_case (since hyphen-case does not work)
* Do add a space before `.`. The property is a word!
    * e.g. `document .body .style .backgroundImage = 'url(doge.png)'`
* Arrow functions with one parameter, take no brackets
* Use `var`, and `var` only
* Try to not mutate `var`s
* No class statements
* Write your unfinished code as `...`
