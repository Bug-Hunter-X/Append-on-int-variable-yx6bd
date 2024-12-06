# Go Bug: Append on int variable

This repository demonstrates a common error in Go: attempting to use the `append` function on an integer variable.

The `append` function is designed to work with slices, not integers.  Attempting to append to an integer will result in a compile-time error.

## Bug

The file `bug.go` contains the erroneous code that attempts to append to an integer.  This code will not compile because of the type mismatch.

## Solution

The file `bugSolution.go` demonstrates the correct way to use the append function. It shows appending elements to a slice of integers.

## How to reproduce

1.  Clone this repository.
2.  Navigate to the directory.
3.  Attempt to compile and run `bug.go`. This will result in a compile-time error.
4.  Compile and run `bugSolution.go`. This will execute successfully, demonstrating the corrected code.

## Lesson Learned

Always ensure the correct type of data is being used with the relevant functions. In this case, `append` is designed to work exclusively with slices.