**scmin** removes unnecessary semicolons from JavaScript.

**scmax** adds unnecessary semicolons to JavaScript.

Based on the Esprima JavaScript parser
([esprima.org](http://esprima.org)).

## Installation

    npm install -g scmin

## Usage

    scmin unnecessary-semicolons.js > lovely.js

    scmax not-enough-semicolons.js > bloated.js

    scmin i-like-pipes.js | scmax > why-not.js

## The fine print

JavaScript's [automatic semicolon
insertion](http://people.mozilla.org/~jorendorff/es5.html#sec-7.9)
allows you to omit semicolons in certain situations.

**scmin** removes semicolons that are unnecessary due to automatic
semicolon insertion.

**scmax** adds semicolons explicit semicolons so that automatic
semicolon insertion is never used.

Both of them preserve whitespace; only semicolons are added or removed.
