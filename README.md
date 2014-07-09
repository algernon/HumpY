HumpY
=====

[![Build Status](https://travis-ci.org/algernon/HumpY.png?branch=master)](https://travis-ci.org/algernon/HumpY)

Ever wanted to use a library in [Hy][hylang], but the library used
ugly CamelCase? Ever wanted to write a wrapper, that converts that
abomination into the One True way of using dashes? Ever thought that
would be a tremendous amount of code for no good reason?

Wonder no more, for all it takes is one clever macro, neatly contained
in this very library!

 [hylang]: http://hylang.org/

Example
-------

```hy
(require humpy.hump)
(import [some.library [camelCase FunctionNames]])

#@camel-case
;; => <function camelCase at 0xdeadbeef>

#@Function-names
;; => <function FunctionNames at 0xdeadbeef>
```

License
-------

All the code is licensed under the GNU Lesser General Public License
(v3+).
