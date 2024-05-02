# Monte Carlo Optimization for Bucket Allocation

This repository contains an implementation of Monte Carlo optimization for allocating items into buckets while minimizing the maximum bucket size.

## Problem Statement

Given a set of items with associated weights, the goal is to distribute these items into buckets in such a way that the maximum bucket size is minimized.

## Input

The input consists of items and their weights, represented as a numpy array:

```python
optMatrix = np.array([
    ['q', 111],
    ['w', 500],
    ['e', 20],
    ['r', 80],
    ['t', 50],
    ['y', 180],
    ['u', 1701],
    ['i', 108],
    ['o', 1780],
    ['p', 18],
    ['a', 10],
    ['s', 178],
    ['d', 10],
    ['g', 109],
    ['h', 1780],
    ['j', 980],
    ['k', 480],
    ['l', 2480],
    ['z', 500],
    ['x', 30]
])


## Output

The output provides the optimal allocation of items into buckets:

```
Bucket 1: [80, 108, 10, 111, 2480]
Bucket 2: [1780, 980]
Bucket 3: [1701, 30, 500, 500, 20]
Bucket 4: [180, 109, 178, 10, 18, 480, 50, 1780]
```