# ctags-xref

This is a fork of Exuberant Ctags intended for C only.  Rather than
generate a proper tags file, this defaults to output unsorted xref
records, with the addition of function end markers.  These are useful
for extracting desired functions from their source files.  A provided
script, show-source, demonstrates how to this may be done.

#### How to build
On Linux and POSIX systems:

	./configure
	make
	make install

#### How to use
To index files in the current directory:

	ctags-xref *.[ch] > index

To index all files in a source tree:

	ctags-xref -R /path/to/source > index

To see a function's source, e.g., createTimer():

	show-source createTimer
