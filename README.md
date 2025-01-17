	=======================================================
	                Quantifier Elimination
	                          in
	            Elementary Algebra and Geometry
	                          by
	      Partial Cylindrical Algebraic Decomposition

	               Version B 1.69, 16 Mar 2012

	                          by
	                       Hoon Hong
	                  (hhong@math.ncsu.edu)

	With contributions by: Christopher W. Brown, George E.
	Collins, Mark J. Encarnacion, Jeremy R. Johnson
	Werner Krandick, Richard Liska, Scott McCallum,
	Nicolas Robidoux, and Stanly Steinberg
	=======================================================
http://www.usna.edu/CS/~qepcad/B/QEPCAD.html


This is a (shallow) fork of QEPCAD, a program performing cylindrical algebraic decomposition.

I found the library a bit hard to build (especially with Visual Studio), so I added CMake files which makes the process considerably easier.

Very Simple Example
-------------------

Given the input

    (Ex)[x^2 + a x + b = 0].

the program will output:

    An equivalent quantifier-free formula:

	4 b - a^2 <= 0

Pretty cool!

There are more examples in the tests folder.

Compiling
=========
With Visual Studio in Windows, everything is included. Just run the CMake graphical interface and point it to the source root.

In Ubuntu, you may have to execute

     sudo apt-get install libreadline-dev 
     
to install a dependency (GNU Readline). Then run

     git clone https://github.com/PetterS/qepcad
     cd qepcad
     mkdir build
     cd build
     cmake ..
     make

