# Common module

This module contains reusable code shared between other modules,
and provides various features.
Here is a list and short description of the header files.


### Configuration.h

Class to retrieve configuration parameters (key/value pairs) from a text file (e.g. .ini format).
This feature is also exported as a Tcl library, libtclConfiguration.so

### Daemon.h

Class to help creating a daemon process running in the background.

### Exceptions.h

Define the exceptions based on boost::exception that we use in the project.

### Iommu.h

Function to check if the IOMMU is enabled.

### Fifo.h

Class implementing  a lock-free 1-to-1 FIFO.
Used to pass data between threads.

### GuardFunction.h

Class that takes a function which is executed on scope exit.

### LineBuffer.h

Class implementing a buffer to read from file descriptor and get out data line by line.

### MakeUnique.h

Provides std::make_unique to c++11. Superseded by C++14, do not use.

### Program.h

Class to help make command-line utilities. Provides options handling, help output, and interrupt handling.

### signalUtilities.h

This file proposes a set of functions to handle signals in your program.
It prints the stack trace when there is a SIGSEV.
It also handles elegantly SIGINT and SIGTERM by catching them and allowing the program
to clean itself up before exiting. If a second SIGINT/SIGTERM is
received before the end of the clean up we exit immediately.

### SimpleLog.h

Class providing simple logging format to a file (or standard output).

### SuffixNumber

Class providing conversions for numbers with a suffix, e.g. 123GB or 42KiB.

### SuffixOption

Class providing SuffixNumber integration for Boost Program Options.

### Thread.h

Class to implement controllable looping threads.

### Timer.h

Class to implement a high resolution timer function.
(counting time or timeout)
