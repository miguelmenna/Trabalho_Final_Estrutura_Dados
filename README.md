# Hash Table and Quick Sort in C

## About the Project

This project implements a data structure based on a **Hash Table**, developed using the C programming language, with the purpose of storing, organizing, searching, and managing collections of names.

The implementation uses doubly linked lists to store elements within buckets, applying the **Separate Chaining** technique to handle hash collisions.

In addition to standard hash table operations, the project incorporates the **Quick Sort** algorithm to sort elements stored in a specific bucket.

The project was developed in an academic context as a practical exercise involving data structures, algorithms, and memory management.

## Technologies and Concepts

- **C Programming Language:** implementation of the application logic and data structures.
- **Hash Table:** data organization and distribution.
- **Separate Chaining:** collision resolution technique.
- **Doubly Linked Lists:** dynamic storage of elements.
- **Quick Sort:** sorting algorithm.
- **ASCII:** character encoding values used by the hash function.
- **File Handling:** reading data from `.txt` files.
- **Dynamic Memory Allocation:** memory management using `malloc()` and `free()`.

## Features

The application provides the following operations:

1. **Insertion:** adds new names to the hash table.
2. **Bucket Statistics:** displays the number of elements stored in each bucket.
3. **Sorting:** sorts and displays the names within a selected bucket using Quick Sort.
4. **Deletion:** removes a specific name from the data structure.
5. **Search:** searches for a specific name in the hash table.
6. **Data Loading:** automatically imports names from the `nomes.txt` file.

## Hash Table Implementation

The data structure uses a total of 23 buckets.

The hash function calculates the sum of the ASCII values of the first five characters of each name. The resulting value is then processed using the modulo operator with 23 as the divisor.

The result determines the bucket where the element is stored.

When multiple names are assigned to the same bucket, collisions are handled using doubly linked lists through the Separate Chaining technique.

## Algorithms and Data Structures

### Hash Table

Used to distribute names across multiple buckets, organizing elements according to their calculated hash values.

### Doubly Linked Lists

Each bucket contains a linked list in which every node maintains references to both the previous and next elements, allowing dynamic data management.

### Quick Sort

Implemented to sort the elements stored within a bucket. The implementation also includes a complementary routine intended to refine sorting based on subsequent characters in the names.

## How to Run

You need a C compiler, such as GCC, installed in your environment.

1. Clone the repository:

```bash
git clone REPOSITORY_URL
```

2. Navigate to the project directory:

```bash
cd PROJECT_NAME
```

3. Make sure the `nomes.txt` file is available in the execution directory.

4. Compile the program:

```bash
gcc main.c -o hash_table
```

5. Run the application:

```bash
./hash_table
```

On Windows, run:

```bash
hash_table.exe
```

**Note:** The original implementation was developed for Windows and uses `system("cls")` to clear the terminal.

## Learning Objectives

This project provided practical experience with fundamental Computer Science concepts, including:

- Implementation of dynamic data structures.
- Hash function development.
- Collision resolution techniques.
- Pointer manipulation and dynamic memory management.
- Sorting algorithm implementation.
- File reading and data processing.
- Data organization and manipulation using C.

## Project Status

Academic project developed in C. The original implementation represents the version created during the learning process and may receive further improvements related to memory safety, input validation, and edge-case handling.
