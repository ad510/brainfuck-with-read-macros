Brainfuck with Read Macros
==========================

The most expressive programming language in the world. Its syntax is so powerful that you can literally turn it into any language you want!

Brainfuck with Read Macros is just like [normal Brainfuck](https://en.wikipedia.org/wiki/Brainfuck), except that if you enter the [magic `!` command](https://esolangs.org/wiki/Brainfuck#Extensions), it will stop parsing your code and feed the rest of the file as input to your Brainfuck program. So if you want to extend the syntax of the language in any way imaginable, all you have to do is write an interpreter for your desired syntax in Brainfuck, then enter the magic `!` command... and bam! Now you're writing code using the new syntax.

See the `examples` folder for sample programs.

Usage
-----
```
gcc -o bfrm bfrm.c
./bfrm filename
```

But those aren't even really [read macros](https://gist.github.com/chaitanyagupta/9324402)!
-------------------------------------------------------------------------------------------
Perhaps, but the language is so expressive that you can implement them as a library.

License
-------
Based on [Krzysztof Gabis's Brainfuck interpreter](https://github.com/kgabis/brainfuck-c) (with some modifications) and licensed under the MIT License.
