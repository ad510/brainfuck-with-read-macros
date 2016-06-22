Brainfuck with Read Macros
==========================

The most expressive programming language in the world. Its syntax is so powerful that you can literally turn it into any language you want!

Brainfuck with Read Macros is just like [normal Brainfuck](https://en.wikipedia.org/wiki/Brainfuck), except that if you enter the magic `!` command, it will stop parsing your code and feed the rest of the file as input to your Brainfuck program. So if you want to extend the syntax of the language in any way imaginable, all you have to do is write an interpreter for your desired syntax in Brainfuck, then enter the magic `!` command... and bam! Now you're writing code using the extended syntax.

See the `examples` folder for sample programs.

**Q: This is [highly unoriginal](https://esolangs.org/wiki/Brainfuck#Extensions), and those aren't even [real read macros](https://gist.github.com/chaitanyagupta/9324402).**

A: I completely agree that Brainfuck with Read Macros is highly unoriginal, but considering that it is the most expressive programming language in the world, I don't think it has been marketed to its full potential. And if you feel that my implementation of read macros is improper, all you have to do is write an interpreter for Brainfuck with "proper" read macros in Brainfuck, and enter the magic `!` command, then any code after that will be able to use "real" read macros!

Usage
-----
```
gcc -o bfrm bfrm.c
./bfrm filename
```

License
-------
Based on [Krzysztof Gabis's Brainfuck interpreter](https://github.com/kgabis/brainfuck-c) (with some modifications) and licensed under the MIT License.
