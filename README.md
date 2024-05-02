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

# isCollection

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Test if a value is a collection.

<section class="intro">

A collection is defined as either an [`Array`][mdn-array], [`Typed Array`][mdn-typed-array], or an array-like [`Object`][mdn-object] (excluding `strings` and `functions`).

</section>

<!-- ./intro -->

<section class="installation">

## Installation

```bash
npm install @womorg/autem-tempora-rem
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm`][esm-url] branch (see [README][esm-readme]).
-   If you are using Deno, visit the [`deno`][deno-url] branch (see [README][deno-readme] for usage intructions).
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd`][umd-url] branch (see [README][umd-readme]).

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

To view installation and usage instructions specific to each branch build, be sure to explicitly navigate to the respective README files on each branch, as linked to above.

</section>

<section class="usage">

## Usage

```javascript
var isCollection = require( '@womorg/autem-tempora-rem' );
```

#### isCollection( value )

Tests if a value is a collection.

```javascript
var bool = isCollection( [] );
// returns true
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint-disable object-curly-newline -->

<!-- eslint no-undef: "error" -->

```javascript
var Int8Array = require( '@stdlib/array-int8' );
var Uint8Array = require( '@stdlib/array-uint8' );
var Uint8ClampedArray = require( '@stdlib/array-uint8c' );
var Int16Array = require( '@stdlib/array-int16' );
var Uint16Array = require( '@stdlib/array-uint16' );
var Int32Array = require( '@stdlib/array-int32' );
var Uint32Array = require( '@stdlib/array-uint32' );
var Float32Array = require( '@stdlib/array-float32' );
var Float64Array = require( '@stdlib/array-float64' );
var isCollection = require( '@womorg/autem-tempora-rem' );

var bool = isCollection( [] );
// returns true

bool = isCollection( new Float64Array( 10 ) );
// returns true

bool = isCollection( new Float32Array( 10 ) );
// returns true

bool = isCollection( new Int32Array( 10 ) );
// returns true

bool = isCollection( new Uint32Array( 10 ) );
// returns true

bool = isCollection( new Int16Array( 10 ) );
// returns true

bool = isCollection( new Uint16Array( 10 ) );
// returns true

bool = isCollection( new Int8Array( 10 ) );
// returns true

bool = isCollection( new Uint8Array( 10 ) );
// returns true

bool = isCollection( new Uint8ClampedArray( 10 ) );
// returns true

bool = isCollection( { 'length': 0 } );
// returns true

bool = isCollection( {} );
// returns false

bool = isCollection( 'beep' );
// returns false

bool = isCollection( isCollection );
// returns false

bool = isCollection( null );
// returns false

bool = isCollection( void 0 );
// returns false

bool = isCollection( 3.14 );
// returns false
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/assert-is-array-like`][@stdlib/assert/is-array-like]</span><span class="delimiter">: </span><span class="description">test if a value is array-like.</span>
-   <span class="package-name">[`@stdlib/assert-is-array-like-object`][@stdlib/assert/is-array-like-object]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object.</span>

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

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@womorg/autem-tempora-rem.svg
[npm-url]: https://npmjs.org/package/@womorg/autem-tempora-rem

[test-image]: https://github.com/womorg/autem-tempora-rem/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/womorg/autem-tempora-rem/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/womorg/autem-tempora-rem/main.svg
[coverage-url]: https://codecov.io/github/womorg/autem-tempora-rem?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/womorg/autem-tempora-rem.svg
[dependencies-url]: https://david-dm.org/womorg/autem-tempora-rem/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/womorg/autem-tempora-rem/tree/deno
[deno-readme]: https://github.com/womorg/autem-tempora-rem/blob/deno/README.md
[umd-url]: https://github.com/womorg/autem-tempora-rem/tree/umd
[umd-readme]: https://github.com/womorg/autem-tempora-rem/blob/umd/README.md
[esm-url]: https://github.com/womorg/autem-tempora-rem/tree/esm
[esm-readme]: https://github.com/womorg/autem-tempora-rem/blob/esm/README.md
[branches-url]: https://github.com/womorg/autem-tempora-rem/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/womorg/autem-tempora-rem/main/LICENSE

[mdn-array]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array

[mdn-typed-array]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/TypedArray

[mdn-object]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object

<!-- <related-links> -->

[@stdlib/assert/is-array-like]: https://github.com/stdlib-js/assert-is-array-like

[@stdlib/assert/is-array-like-object]: https://github.com/stdlib-js/assert-is-array-like-object

<!-- </related-links> -->

</section>

<!-- /.links -->
