# Sorting Algorithms: Time and Space Comparison

**Course:** Analysis of Algorithms | **Assignment 3**
**Student:** Fawaz Naseer (SAP ID: 59028)

## About
This project compares four sorting algorithms, written from scratch in Python:

- Selection Sort
- Bubble Sort
- Quick Sort (last element as pivot)
- Merge Sort

Each algorithm is tested on 4 arrays, which gives 16 runs in total:

| Case | Array size | Order |
|------|-----------|-------|
| 1 | 5 | Sorted |
| 2 | 5 | Reverse sorted |
| 3 | 100 | Sorted |
| 4 | 100 | Reverse sorted |

## What is recorded
For every run the notebook records:
- **Time:** 3 timed runs and their average, in microseconds (µs). Each timed run sorts 500 fresh copies of the array and divides by 500, so very small times can be measured. Copying is not included in the timing.
- **Comparisons:** the number of comparisons the algorithm makes.
- **Extra memory:** peak extra memory in bytes (measured with `tracemalloc`).
- **Recursion depth:** the deepest recursion level reached (shows stack space for Quick Sort and Merge Sort).

## How to run
1. Open `Sorting_Assignment3.ipynb` in [Google Colab](https://colab.research.google.com) (File > Upload notebook).
2. Click **Runtime > Run all**.
3. The notebook checks each algorithm against Python's `sorted()`, then prints one results table per case and saves them as CSV files.

No extra installation is needed. Python 3, `pandas`, and the standard library are enough (all are already available in Colab).

## Files
- `Sorting_Assignment3.ipynb`: the source code and experiments
- `table_case1.csv` to `table_case4.csv`: the result tables for the 4 cases

## Note
Timings depend on the machine and on how busy it is, so running the notebook again will give slightly different times. The comparison counts and recursion depths are always the same.
