Understand:
- Time Complexity of Sorting Algorithms
- Stable or not. Stable sorting means that if two elements have equal value, their original order is preserved in the sorted output.
- In-place sorting or not. No memory for additional data structure to store intermediate results.

## Insertion Sort

```python
def insertion_sort(unsorted_lst: list) -> list:
    n = len(unsorted_lst)
    for i in range(n):
        curr = i
        while curr > 0 and unsorted_lst[curr] < unsorted_lst[curr-1]:
            unsorted_lst[curr-1], unsorted_lst[curr] = unsorted_lst[curr], unsorted_lst[curr-1]
            curr -= 1
    return unsorted_lst
```