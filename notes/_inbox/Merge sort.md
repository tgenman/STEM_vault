---
aliases:
  - Сортировка слиянием
publish: true
anki: false
created: 2024-05-23 12:52
parent: 
connected:
  - "#обс/linking"
tags:
  - empty
---

$$O(n*log(n))$$


![[Pasted image 20240523125223.png|300]]

```python
def merge_sort(container):
    size = len(container)
    if size == 1:
        return container
    elif size == 2:
        return sorted(container)
    else:
        half = int(size / 2)
        return __merge_sort_pair__(merge_sort(container[:half]), merge_sort(container[half:]))
    
    
def __merge_sort_pair__(one, two):
    result = []
    size_one = len(one)
    size_two = len(two)
    index_one = 0
    index_two = 0
    
    for _ in range(size_one + size_two):
        if index_one == size_one:
            result.append(two[index_two])
            index_two += 1

        elif index_two == size_two:
            result.append(one[index_one])
            index_one += 1

        elif one[index_one] <= two[index_two]:
            result.append(one[index_one])
            index_one += 1

        else:
            result.append(two[index_two])
            index_two += 1
    
    return result
```