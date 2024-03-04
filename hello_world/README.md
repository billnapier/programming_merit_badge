## Hello World Examples.

A program that does nothing more than say "Hello World!" is the canonical starting program in any language.  This directory contains a few examples that may help you get started on Requirements 5b and 5c.

Running any of these is going to be easiest from a terminal.  Two ways in Codepsaces to get a terminal: 

1. Ctrl + Shift + `
1. Use the command palette: Ctrl + Shift + P and then type "new terminal" and pick it from the menu.

I can never remember the keystrokes, so I always use the Command Palette.  Anything and Everything you can do from VSCode can be found there.

### C plus plus (CPP)

C++ is a compiles language, so we need to call "g++" (which is part of the gcc toolchain to compile c++ code).  This complier outputs a file called (by default) `a.out`.  We can then run that new binary to see our output.

```bash
$ cd hello_world/cpp
$ g++ hello_world.cpp
$ ./a.out
```

### Golang (or just go)

Also a compiled language, but has a lot of things to make the compile step easier for you.  We're going to use `go run` to both compile and run the command.

```bash
$ cd hello_world/golang
$ go run hello_world.go
```

### Java

Also a compiled language (remember we talked about it compliing to Java Bytecode?).  Anyway, you can run `javac` to compile the program, and then run `java` to fire up the JVM to execute the bytecode.

```bash
$ cd hello_world/java
$ javac HelloWorld.java
$ java HelloWorld
```

### Python

Python is a scripting language, so doesn't require a compiler.  As an implementation detail, it happens to do a compile before it runs your script, and you can sometimes see the compiled `.pyc` files in your directory after you've run them.

```bash
$ cd hello_world/python
$ python3 hello_world.py
```