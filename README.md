# Algorithm Assignment — Merge Sort vs. Radix Sort

Analysis and implementation of two sorting algorithms, comparing their design, complexity, and performance.

## Overview

This assignment implements **Merge Sort** and **Radix Sort** in Python, analyzes the time complexity of each step, and compares the two algorithms on stability, efficiency with large datasets, and sensitivity to the number of digits in the data.

## Algorithms

### Merge Sort
- Divide-and-conquer: splits the array in half, recursively sorts each half, then merges the two sorted halves.
- Time complexity: **O(n log n)**

### Radix Sort
- Non-comparison sort: sorts numbers digit by digit using a stable counting sort as a subroutine.
- Time complexity: **O(n · d)**, where `d` is the number of digits in the largest element

## Comparison

- **Stability**: Both algorithms are stable.
- **Large datasets**: Radix sort tends to perform better on large datasets of fixed-length numbers.
- **Number of digits**: Radix sort is preferable when the number of digits is smaller than `log n`; merge sort is preferable otherwise.

## Files

- `merge_sort.ipynb` — merge sort implementation and test run
- `radix-2.ipynb` — radix sort implementation and test run
- `Algorithm Assignment.docx` — pseudocode, complexity analysis, and comparison write-up

## Running It

Open either notebook in Jupyter and run all cells:

```bash
jupyter notebook merge_sort.ipynb
jupyter notebook radix-2.ipynb
```

## Note

This project was built for a university algorithms course, to compare a comparison-based sort against a non-comparison-based sort on the same input.
