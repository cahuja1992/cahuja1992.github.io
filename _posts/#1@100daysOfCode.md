---
  layout:     post
  title:      #100daysOfCode: #1 Two Number Sum @ Arrays 
  date:       2020-07-08
  summary:    Evaluation questions for participating students in the course (Fundamentals to Data Crunching)
  categories: Courses/Computer Science/Algorithms
  cover-image: /images/post_12/thumbnail.png
---
![Deep Learning](images/../../images/post_12/dl_poster.jpg)

### 1. Two Number Sum

Write a function that takes in a non-empty array of distinc integers and an integer representing a target sum. If any two numbers in the input array sum upto the target sum, the function should return them in an array, in any order. If no two numbers sum up to the target sum, the function should return an empty array. 

Note that the target sum hass to be obtained by summing two different integers in the array; you can't add a single integer to itself in order to obtain the target sum.

You can assume that there will be at most one pair of numbers summing up to the target sum.

**Input**
```
array = [3, 5, -4, 8, 11, 1, -1, 6]
targetSum = 10
```
**Output**
```
[-1, 11] // the numbers could be in reverse order
```

**NOTE:** Optimal Solution: O(n) time | O(n) space - where n is the length of the input array.
