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
```


## Output

The output provides the optimal allocation of items into buckets:

```
Bucket Cost - [  10  178 2480  109] Elements - ['d' 's' 'l' 'g']
Bucket Cost - [  30 1701   20   10  980] Elements - ['x' 'u' 'e' 'a' 'j']
Bucket Cost - [ 500  480 1780] Elements - ['z' 'k' 'o']
Bucket Cost - [  18  108   80   50  111  180 1780  500] Elements - ['p' 'i' 'r' 't' 'q' 'y' 'h' 'w']
```
