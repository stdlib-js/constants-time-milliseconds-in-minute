<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# Milliseconds in a Minute

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Number of milliseconds in a minute.



<section class="usage">

## Usage

To use in Observable,

```javascript
MILLISECONDS_IN_MINUTE = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/constants-time-milliseconds-in-minute@umd/browser.js' )
```
The previous example will load the latest bundled code from the umd branch. Alternatively, you may load a specific version by loading the file from one of the [tagged bundles](https://github.com/stdlib-js/constants-time-milliseconds-in-minute/tags). For example,

```javascript
MILLISECONDS_IN_MINUTE = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/constants-time-milliseconds-in-minute@v0.3.3-umd/browser.js' )
```

To vendor stdlib functionality and avoid installing dependency trees for Node.js, you can use the UMD server build:

```javascript
var MILLISECONDS_IN_MINUTE = require( 'path/to/vendor/umd/constants-time-milliseconds-in-minute/index.js' )
```

To include the bundle in a webpage,

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/constants-time-milliseconds-in-minute@umd/browser.js"></script>
```

If no recognized module system is present, access bundle contents via the global scope:

```html
<script type="text/javascript">
(function () {
    window.MILLISECONDS_IN_MINUTE;
})();
</script>
```

#### MILLISECONDS_IN_MINUTE

Number of milliseconds in a minute.

```javascript
var bool = ( MILLISECONDS_IN_MINUTE === 60000 );
// returns true
```

</section>

<!-- /.usage -->

<section class="notes">

## Notes

-   The value is a generalization and does **not** take into account inaccuracies arising due to complications with time and dates.

</section>

<!-- /.notes -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/random-base-randu@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-roundn@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/constants-time-milliseconds-in-minute@umd/browser.js"></script>
<script type="text/javascript">
(function () {

var ms;
var m;
var i;

function mins2ms( mins ) {
    return mins * MILLISECONDS_IN_MINUTE;
}

for ( i = 0; i < 10; i++ ) {
    m = roundn( randu()*20.0, -2 );
    ms = mins2ms( m );
    console.log( '%d mins => %d milliseconds', m, ms );
}

})();
</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2026. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/constants-time-milliseconds-in-minute.svg
[npm-url]: https://npmjs.org/package/@stdlib/constants-time-milliseconds-in-minute

[test-image]: https://github.com/stdlib-js/constants-time-milliseconds-in-minute/actions/workflows/test.yml/badge.svg?branch=v0.3.3
[test-url]: https://github.com/stdlib-js/constants-time-milliseconds-in-minute/actions/workflows/test.yml?query=branch:v0.3.3

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/constants-time-milliseconds-in-minute/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/constants-time-milliseconds-in-minute?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/constants-time-milliseconds-in-minute.svg
[dependencies-url]: https://david-dm.org/stdlib-js/constants-time-milliseconds-in-minute/main

-->

[chat-image]: https://img.shields.io/badge/zulip-join_chat-brightgreen.svg
[chat-url]: https://stdlib.zulipchat.com

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/constants-time-milliseconds-in-minute/tree/deno
[deno-readme]: https://github.com/stdlib-js/constants-time-milliseconds-in-minute/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/constants-time-milliseconds-in-minute/tree/umd
[umd-readme]: https://github.com/stdlib-js/constants-time-milliseconds-in-minute/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/constants-time-milliseconds-in-minute/tree/esm
[esm-readme]: https://github.com/stdlib-js/constants-time-milliseconds-in-minute/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/constants-time-milliseconds-in-minute/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/constants-time-milliseconds-in-minute/main/LICENSE

</section>

<!-- /.links -->
