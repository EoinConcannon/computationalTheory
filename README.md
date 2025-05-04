# computationalTheory

- Required repository for "Computational Theory" course.
- Notes and Assessment page here: https://github.com/ianmcloughlin/computational_theory

## Table of Contents
- [Module Overview](#module-overview)
- [Getting Started](#getting-started)
- [Tasks](#tasks)
  - [Task 1: Binary Representations](#task-1-binary-representations)
  - [Task 2: Hash Functions](#task-2-hash-functions)
  - [Task 3: SHA256](#task-3-sha256)
  - [Task 4: Prime Numbers](#task-4-prime-numbers)
  - [Task 5: Roots](#task-5-roots)
  - [Task 6: Proof of Work](#task-6-proof-of-work)
  - [Task 7: Turing Machines](#task-7-turing-machines)
  - [Task 8: Computational Complexity](#task-8-computational-complexity)

## Module Overview

This repository serves as a comprehensive exploration of computational theory concepts, implemented and demonstrated using Python. It is designed to provide hands-on experience with fundamental topics in computer science, ranging from binary operations and cryptographic algorithms to Turing machines and computational complexity. Each concept is presented as a task within a Jupyter notebook, allowing for interactive learning and experimentation.

The module covers a wide array of topics, including:

- **Binary Representations**: Understanding and manipulating binary data, a cornerstone of computer science.
- **Hash Functions**: Exploring the principles of hashing, including custom implementations and their applications in data integrity and cryptography.
- **SHA256**: Delving into the mechanics of the SHA256 cryptographic hash function, including its padding requirements and use cases.
- **Prime Numbers**: Investigating prime number generation and their significance in cryptography and number theory.
- **Mathematical Roots**: Calculating constants derived from mathematical roots, often used in cryptographic algorithms.
- **Proof of Work**: Simulating a simplified proof-of-work system, a key concept in blockchain technology.
- **Turing Machines**: Implementing a Turing machine to understand the theoretical foundations of computation.
- **Computational Complexity**: Analyzing the performance of algorithms, with a focus on sorting and its computational implications.

## Getting Started

To run these tasks:

1. Clone this repository
2. Install required dependencies: `pip install -r requirements.txt` (if needed)
3. Open `tasks.ipynb` in Jupyter Notebook or Jupyter Lab
4. Execute the cells to see the examples in action

## Tasks

### Task 1: Binary Representations
This task involves implementing functions to manipulate binary representations of numbers:
- `rotl(x, n)`: Rotates the bits of a 32-bit unsigned integer `x` to the left by `n` positions.
- `rotr(x, n)`: Rotates the bits of a 32-bit unsigned integer `x` to the right by `n` positions.
- `ch(x, y, z)`: A bitwise function used in cryptographic hash functions.
- `maj(x, y, z)`: Another bitwise function used in cryptographic hash functions.

### Task 2: Hash Functions
This task demonstrates the implementation of a simple hash function:
- A C-style hash function is implemented in Python to compute a hash value for a string.
- The hash function uses modular arithmetic to ensure the hash value fits within a fixed range.

### Task 3: SHA256
This task involves implementing the padding step of the SHA256 cryptographic hash function:
- Reads a file and calculates the padding required to make the file's size a multiple of 512 bits.
- Outputs the padded message in hexadecimal format.

### Task 4: Prime Numbers
This task explores prime number generation and verification:
- Implements methods to check if a number is prime.
- Generates the first `n` prime numbers.
- Extracts the first 32 bits of the fractional part of the square root of each prime number.

### Task 5: Roots
This task involves working with mathematical roots:
- Computes the first 32 bits of the fractional part of the square root of a number.
- Uses this computation to generate constants for cryptographic applications.

### Task 6: Proof of Work
This task demonstrates a proof-of-work system:
- Computes the SHA256 hash of words from a dictionary.
- Finds the word with the most leading zero bits in its hash.
- Outputs the word and the number of leading zero bits as proof.

### Task 7: Turing Machines
This task involves simulating a Turing Machine:
- Implements a Turing Machine that adds 1 to a binary number on its tape.
- The machine starts at the left-most non-blank symbol and treats the right-most symbol as the least significant bit.

### Task 8: Computational Complexity
This task demonstrates the computational complexity of sorting algorithms:
- Implements a modified Bubble Sort algorithm that counts the number of comparisons made during sorting.
- Sorts all permutations of a list and outputs the number of comparisons required for each permutation.