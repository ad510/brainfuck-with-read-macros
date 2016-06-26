Brainfuck with Read Macros
==========================

The most expressive programming language in the world. Its syntax is so powerful that you can literally turn it into any language you want!

Brainfuck with Read Macros is just like [normal Brainfuck](https://en.wikipedia.org/wiki/Brainfuck), except that if you enter the [magic `!` command](https://esolangs.org/wiki/Brainfuck#Extensions), it will stop parsing your code and feed the rest of the file as input to your Brainfuck program. So if you want to extend the syntax of the language in any way imaginable, all you have to do is write an interpreter for your desired syntax in Brainfuck, then enter the magic `!` command... and bam! Now you're writing code using the new syntax.

See the `examples` folder for sample programs.

Usage
-----
```
g++ -O3 -o bfrm bfrm.cc
./bfrm filename
```

But those aren't even really [read macros](https://gist.github.com/chaitanyagupta/9324402)!
-------------------------------------------------------------------------------------------
Perhaps, but the language is so expressive that you can implement them as a library.

Acknowledgement
---------------
This is based on [Shinichiro Hamaji's work](https://github.com/shinh/bflisp) of running a Lisp interpreter on Brainfuck.

Copying
-------
Written in 2016 by Andrew Downing

To the extent possible under law, the author(s) have dedicated all copyright and related and neighboring rights to this software to the public domain worldwide. This software is distributed without any warranty.

You should have received a copy of the CC0 Public Domain Dedication along with this software. If not, see <http://creativecommons.org/publicdomain/zero/1.0/>.
