# Foothread Library and ComputeSum Application

## Overview

This project implements a custom user-level thread library called `foothread`, designed as part of the CS39002 Operating Systems Laboratory course at IIT Kharagpur. The library provides basic threading capabilities similar to `pthread`, along with mutexes and barriers for synchronization, but is implemented from scratch without relying on existing thread libraries like `pthread` or `OpenMP`. Additionally, a sample application `computesum` is provided to demonstrate the usage of the `foothread` library.

## Files

- **foothread.h**: Header file containing the declarations and necessary macros for the `foothread` library.
- **foothread.c**: Implementation file for the `foothread` library, containing definitions for thread creation, termination, mutexes, and barriers.
- **computesum.c**: An application that utilizes the `foothread` library to compute the sum of values entered at the leaf nodes of a tree structure.
- **gentree.c**: A utility to generate random tree structures, used as input for the `computesum` application.
- **tree.txt**: Sample input file storing the parent representation of a tree.

## Compilation and Execution

### Build the Library

To compile and create the `foothread` dynamic library:

```bash
make lib
```

## Compile the Application
To compile the computesum application:

```bash
make app
```

## Run the Application
To run the computesum application with a provided tree.txt file:

```bash
make run
```

## Generate a New Tree
To generate a new random tree and run the application:

```bash
make newrun
``` 

## Clean Up
To clean up the compiled binaries and object files:

```bash
make clean
```
## Usage
The `computesum` application reads a tree structure from tree.txt, prompts the user to enter values at the leaf nodes, and calculates the sum at the root node using the foothread library. The library handles thread creation, synchronization using mutexes and barriers, and ensures correct execution without relying on any existing thread libraries.
