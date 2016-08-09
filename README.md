Brainfuck with Read Macros
==========================

The most expressive programming language in the world. Its abstractions are so powerful that you can literally turn it into any language you want!

Brainfuck with Read Macros is just like [normal Brainfuck](https://en.wikipedia.org/wiki/Brainfuck), except that if you enter the [magic `!` command](https://esolangs.org/wiki/Brainfuck#Extensions), it will stop parsing your code and feed the rest of the file as input to your Brainfuck program. So if you want to extend the syntax of the language in any way imaginable, all you have to do is write an interpreter for your desired syntax in Brainfuck, then enter the magic `!` command... and bam! Now you're writing code using the new syntax.

See the `examples` folder for sample programs, including [FizzBuzz in Lisp syntax](https://raw.githubusercontent.com/ad510/brainfuck-with-read-macros/master/examples/fizzbuzz_lisp.bfrm).

Usage
-----
```
g++ -O3 -o bfrm bfrm.cc
./bfrm filename
```

But it's too slow!
------------------
Maybe it is now, but it won't be after I write a sufficiently smart compiler!

But it doesn't have "real" [read macros](https://gist.github.com/chaitanyagupta/9324402) or [insert abstraction here]!
----------------------------------------------------------------------------------------------------------------------
But guess what? The language is so expressive that you can implement those abstractions as a library! Arguably, that's even better than if they're built into the language because then you can do [bottom-up programming](http://paulgraham.com/progbot.html). Isn't that cool?

But how do I import libraries?
------------------------------
The idiomatic way to do this is to write a package manager that inputs a list of dependencies, downloads them all, and outputs a Brainfuck with Read Macros file with all the dependencies embedded in it so that you can just write your new code at the bottom of the file. That may seem inelegant, but even in a "normal" importing system, you still have to download the dependencies anyway -- they'd just be in separate files instead of the same file as your program. And when every program comes with its dependencies, it means you will never have a [left-pad fiasco](http://m.theregister.co.uk/2016/03/23/npm_left_pad_chaos/).

That said, if we extend the concept of "the most expressive programming language in the world" to include writing programs across multiple files, then just about every programming language in use today would already be the most expressive programming language in the world. How? Instead of writing an interpreter at the top of the file, entering the magic command, then writing code in any language you want, you instead write an interpreter in one file that runs code from another file, and the code in that other file can be written in any language you want!

Acknowledgement
---------------
This is based on [Shinichiro Hamaji's work](https://github.com/shinh/bflisp) of running a Lisp interpreter on Brainfuck.

Copying
-------
Written in 2016 by Andrew Downing

To the extent possible under law, the author(s) have dedicated all copyright and related and neighboring rights to this software to the public domain worldwide. This software is distributed without any warranty.

You should have received a copy of the CC0 Public Domain Dedication along with this software. If not, see <http://creativecommons.org/publicdomain/zero/1.0/>.
