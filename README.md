# ctags-xref

This is a fork of Exuberant Ctags intended for C only.  Rather than
generate a proper tags file, this defaults to output unsorted xref
records, with the addition of function end markers.  These are useful
for extracting desired functions from their source files.

#### How to build
On Linux and POSIX systems:

	./configure
	make
	make install
