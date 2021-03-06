# com.lemonodor/xio

[![Build Status](https://travis-ci.org/wiseman/clj-xio.png?branch=master)](https://travis-ci.org/wiseman/clj-xio) [![Coverage Status](https://coveralls.io/repos/wiseman/clj-xio/badge.png?branch=master)](https://coveralls.io/r/wiseman/clj-xio?branch=master)

```
[com.lemonodor/xio "0.2.3"]
```

Extra IO functions for Clojure. I wrote these soon after I learned
clojure so they're probably an incorrect implementation of a bad idea.


## copy

`xio/copy` is like `clojure.core/copy` but supports the `:callback` option.


## slurp

`xio/slurp` is like `clojure.core/slurp` but is buffered and supports
the `:callback` option. 2.9x faster than `clojure.core/slurp` when
reading a 100 KB file, 3.4x faster when reading a 1 MB file.

## spit

`xio/spit` is like `clojure.core/spit` but is buffered and supports
the `:callback` option.


## binary-slurp

Like `clojure.core/slurp` but returns a byte array.

## binary-spit

## Running tests

To run unit tests:

```
$ lein test
```

To run benchmarks:

```
$ lein test :benchmark
```

## License

Copyright © 2014,2016 John Wiseman

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.
