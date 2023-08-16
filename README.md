# Insertion Sort Algorithm

The given repository contains of an implementation of the Insertion Sort algorithm in a pseudocode-like format. Insertion Sort is a simple comparison-based sorting algorithm that builds the final sorted array one element at a time.

## Algorithm Overview

The `InsertionSort` algorithm works by iterating through an array of elements and repeatedly moving an element into its correct position within the sorted portion of the array.

1. Start with the second element (index 1) and compare it with the previous elements in the sorted part of the array.
2. If the current element is smaller, shift the larger elements to the right to make space for the current element.
3. Insert the current element in its correct position within the sorted part of the array.

## Pseudocode

```plaintext
ALGORITHM InsertionSort
VAR
    array: an array of elements to be sorted
    n: the number of elements in the array
BEGIN
    FOR i <- 1 TO n-1
        key <- array[i]
        j <- i - 1
        WHILE j >= 0 AND array[j] > key
            array[j + 1] <- array[j]
            j <- j - 1
        ENDWHILE
        array[j + 1] <- key
    ENDFOR
END
