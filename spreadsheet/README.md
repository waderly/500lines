# Web Spreadsheet in 99 Lines

    Author: Audrey Tang
    Languages: JS (ES6), HTML5, CSS3
    Dependencies: AngularJS, Web Workers, Traceur Compiler
    Alternatives: ReactJS, LiveScript, JS (ES5)

## Chapter Text

* English: <https://github.com/audreyt/500lines/blob/master/spreadsheet/chapter.md>
* 中文: <https://github.com/audreyt/500lines/blob/master/spreadsheet/chapter.zh-tw.md>

## Online Demo

* ES6 (gh-pages): <http://audreyt.github.io/500lines/spreadsheet/>
* ES5 (jsFiddle): <http://jsfiddle.net/audreyt/LtDyP/>

## Local Demo

Simply open `index.html` with Firefox, Safari or IE11+, and enter some content.

Values starting with `=` are parsed as formula written in JavaScript, for example `=A1*C1`.

If you'd like to use Chrome, type `make run` or `node extra/static-here.js` and connect to [localhost:8888](http://127.0.0.1:8888/) to view the demo.

## Building the Code

To build from source, first install [NodeJS](http://www.nodejs.org/) 0.10 or later, and run `make` (only tested on Linux/OSX at the moment).

JS source code (`main.js` and `worker.js`) are written in ECMAScript 6 (aka _ES.next_, aka _Harmony_), specifically the subset marked with [TC39 Consensus](https://developer.mozilla.org/en-US/docs/Web/JavaScript/ECMAScript_6_support_in_Mozilla) as of February 2014.

For backward compatibility with ECMAScript 5 browsers, we use [Traceur](https://github.com/google/traceur-compiler) to compile source files into the `es5/` directory.

If you prefer to work directly with the 2010 edition of JS, the [as-javascript-1.8.5](https://audreyt.github.io/500lines/spreadsheet/as-javascript-1.8.5/) directory has **main.js** and **worker.js** written in the style of ES5; the [source code](https://github.com/audreyt/500lines/tree/master/spreadsheet/as-javascript-1.8.5) is line-by-line comparable to the ES6 version with the same line count.

For people preferring a cleaner syntax, the [as-livescript-1.2.0](https://audreyt.github.io/500lines/spreadsheet/as-livescript-1.2.0/) directory uses [LiveScript](http://livescript.net/) instead of ES6 to write **main.ls** and **worker.ls**; the [source code](https://github.com/audreyt/500lines/tree/master/spreadsheet/as-livescript-1.2.0) is 20 lines shorter than the JS version.

Building on the LiveScript language, the [as-react-livescript](https://audreyt.github.io/500lines/spreadsheet/as-react-livescript/) directory uses the [ReactJS](https://facebook.github.io/react/) framework; the [source code](https://github.com/audreyt/500lines/tree/master/spreadsheet/as-react-livescript) is 10 lines more than the AngularJS equivalent, but runs considerably faster.

For the version without AngularJS version, using only basic ES5 and raw DOM APIs, the [source code](https://github.com/audreyt/500lines/tree/master/spreadsheet/as-without-angularjs) still clocks at 99 lines, albeit with some short statements joined together.

# CC0 1.0 Universal

To the extent possible under law, 唐鳳 has waived all copyright
and related or neighboring rights to "Web Spreadsheet in 99 Lines".

This work is published from Taiwan.

http://creativecommons.org/publicdomain/zero/1.0
