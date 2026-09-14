---
aliases:
  - Сортировка выбором
created: 2024-05-23 12:49
parent:
  - "[[510.5 🐜Algorithms MOC]]"
connected:
---

$$O(n^2)$$

![[Pasted image 20240523125053.png|300]]

```python
def selection_sort(lst):
    if len(lst) == 1:
        return lst
    for i in range(len(lst)):
        smallest_pointer = i
        for j in range(i+1, len(lst)):
            if lst[j] < lst[smallest_pointer]:
                smallest_pointer = j
        lst[i], lst[smallest_pointer] = lst[smallest_pointer], lst[i]
    return lst

```
