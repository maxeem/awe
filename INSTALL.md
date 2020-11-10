# INSTALLING AWE


## Requirements

A Debian-like operating system, Gnu C, Python 2, OCaml 4.05 or later, make, ar and the Boehm GC.

On Windows use the Windows 10 Linux Subsystem.

Install the packages:

     gcc ocaml-nox python2 binutils libgc-dev


## Building Awe

These are commands to compile and install Awe, to be run from within
the "awe/" source code directory:

`make`

   This builds Awe, then performs a large number of automated tests on it.

`sudo make install`

   This installs Awe. 

   The default destination is the standard "/usr/local" directories.
   Edit Makefile if you do not want this.

`man awe`

   Learn how to run your new Algol W compiler.

That's it, it should be that simple.

Feel free to ask me any questions. 
My email address is in the distribution file.

---
Glyn Webster, 2020