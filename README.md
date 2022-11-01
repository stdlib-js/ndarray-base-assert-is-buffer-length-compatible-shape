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

# isBufferLengthCompatibleShape

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Determine if a buffer length is compatible with an array shape.

<!-- Section to include introductory text. Make sure to keep an empty line after the intro `section` element and another before the `/section` close. -->

<section class="intro">

</section>

<!-- /.intro -->

<!-- Package usage documentation. -->



<section class="usage">

## Usage

<!-- eslint-disable id-length -->

```javascript
import isBufferLengthCompatibleShape from 'https://cdn.jsdelivr.net/gh/stdlib-js/ndarray-base-assert-is-buffer-length-compatible-shape@deno/mod.js';
```

#### isBufferLengthCompatibleShape( len, shape )

Returns a `boolean` indicating if a buffer `length` is compatible with a provided `shape` array.

<!-- eslint-disable id-length -->

```javascript
var shape = [ 2, 2 ];

var bool = isBufferLengthCompatibleShape( 10, shape );
// returns true

bool = isBufferLengthCompatibleShape( 3, shape );
// returns false
```

</section>

<!-- /.usage -->

<!-- Package usage notes. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="notes">

</section>

<!-- /.notes -->

<!-- Package usage examples. -->

<section class="examples">

## Examples

<!-- eslint-disable id-length -->

<!-- eslint no-undef: "error" -->

```javascript
import discreteUniform from 'https://cdn.jsdelivr.net/gh/stdlib-js/random-base-discrete-uniform@deno/mod.js';
import isBufferLengthCompatibleShape from 'https://cdn.jsdelivr.net/gh/stdlib-js/ndarray-base-assert-is-buffer-length-compatible-shape@deno/mod.js';

var shape;
var bool;
var len;
var i;

len = 500; // buffer length

shape = [ 0, 0, 0 ];
for ( i = 0; i < 100; i++ ) {
    // Generate a random array shape:
    shape[ 0 ] = discreteUniform( 1, 10 );
    shape[ 1 ] = discreteUniform( 1, 10 );
    shape[ 2 ] = discreteUniform( 1, 10 );

    // Determine if the buffer length is compatible with the shape array:
    bool = isBufferLengthCompatibleShape( len, shape );
    console.log( 'Buffer length: %d. Shape: %s. Compatible: %s.', len, shape.join( 'x' ), bool );
}
```

</section>

<!-- /.examples -->

<!-- Section to include cited references. If references are included, add a horizontal rule *before* the section. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="references">

</section>

<!-- /.references -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2022. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/ndarray-base-assert-is-buffer-length-compatible-shape.svg
[npm-url]: https://npmjs.org/package/@stdlib/ndarray-base-assert-is-buffer-length-compatible-shape

[test-image]: https://github.com/stdlib-js/ndarray-base-assert-is-buffer-length-compatible-shape/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/ndarray-base-assert-is-buffer-length-compatible-shape/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/ndarray-base-assert-is-buffer-length-compatible-shape/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/ndarray-base-assert-is-buffer-length-compatible-shape?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/ndarray-base-assert-is-buffer-length-compatible-shape.svg
[dependencies-url]: https://david-dm.org/stdlib-js/ndarray-base-assert-is-buffer-length-compatible-shape/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/ndarray-base-assert-is-buffer-length-compatible-shape/tree/deno
[umd-url]: https://github.com/stdlib-js/ndarray-base-assert-is-buffer-length-compatible-shape/tree/umd
[esm-url]: https://github.com/stdlib-js/ndarray-base-assert-is-buffer-length-compatible-shape/tree/esm
[branches-url]: https://github.com/stdlib-js/ndarray-base-assert-is-buffer-length-compatible-shape/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/ndarray-base-assert-is-buffer-length-compatible-shape/main/LICENSE

</section>

<!-- /.links -->
