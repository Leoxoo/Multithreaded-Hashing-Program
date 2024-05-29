## Overview
This program calculates the Jenkins hash of a file using a multithreaded approach with a binary tree structure. The program leverages memory mapping and threads to process file blocks simultaneously, ensuring efficient computation.

## Files
- ho.c: Main program file containing the implementation.
- common.h: Utility functions for timing and spinning.
- common_threads.h: Wrapper functions for pthread operations to ensure error checking.

## Features
- Multithreaded execution using a binary tree structure.
- Memory mapping for efficient file access.
- Recursive thread creation to compute hashes.
- Robust error handling and memory management.
  
## Build Instructions
To compile the program, run the following command:
~~~
gcc -o hash_calculator ho.c -lpthread
~~~
## Usage
To run the program, use the following command:
~~~
./hash_calculator <filename> <numThreads>
~~~
< filename >: Path to the file to be hashed.

< numThreads >: Number of threads to use for hashing.
