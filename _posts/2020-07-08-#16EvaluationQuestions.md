---
  layout:     post
  title:      Course: Fundamentals to Data Crunching (Student Evaluation)
  date:       2020-07-08
  summary:    Evaluation questions for participating students in the course (Fundamentals to Data Crunching)
  categories: Courses/Computer Science/Algorithms
  cover-image: /images/post_12/thumbnail.png
---
![Deep Learning](images/../../images/post_12/dl_poster.jpg)
Following are the question that helps me to understand where all of you stand in terms of your breadth and knowledge of Data Structure and Algorithms and thus, I can stress more on the areas where I feel you all need more guidance.

## Q1: Swap Alternate (Evaluate)

You have been given an array/list of size N. You need to swap every pair of alternate elements in the array/list.
You don't need to print or return anything, just change in the input array itself.

**Input Format :**
```The first line contains an Integer 't' which denotes the number of test cases or queries to be run. Then the test cases follow.

First line of each test case or query contains an integer 'N' representing the size of the array/list.

Second line contains 'N' single space separated integers representing the elements in the array/list.
```

**Output Format :**
```
For each test case, print the elements of the resulting array in a single row separated by a single space.

Output for every test case will be printed in a separate line.
```


**Constraints :**
```
1 <= t <= 10^2
0 <= N <= 10^5
Time Limit: 1sec
```


**Sample Input 1:**
```
1
6
9 3 6 12 4 32
```
**Sample Output 1 :**
```
3 9 12 6 32 4
```

**Sample Input 2:**
```
2
9
9 3 6 12 4 32 5 11 19
4
1 2 3 4
```
**Sample Output 2 :**
```
3 9 12 6 32 4 11 5 19 
2 1 4 3 
```



## Q2: Count platforms

Given two arrays (both of size n), one containing arrival time of trains and other containing the corresponding trains departure time (in the form of an integer) respectively. Return the minimum number of platform required, such that no train waits.
Arrival and departure time of a train can't be same.
**Input Format :**
```
Line 1: Integer n, number of elements in arrival and departure array
Line 2: Elements of Arrival Array (separated by spaces).
Line 3: Elements of Departure Array (separated by spaces).
```
**Output Format:**
```
Minimum Number of Platform Needed
```
**Constraints :**
```
1 <= n <= 100
```
**Sample Input 1 :**
```
6
900 940 950 1100 1500 1800
910 1200 1120 1130 1900 2000
```
**Sample Output 1 :**
```
3
```
**Sample Input 2 :**
```
4
1100 1101 1103 1105
1110 1102 1104 1106
```
**Sample Output 2 :**
```
2
```



## Q3: Maximum Profit on App (Evaluate)

You have made a smartphone app and want to set its price such that the profit earned is maximised. There are certain buyers who will buy your app only if their budget is greater than or equal to your price.
You will be provided with a list of size N having budgets of buyers and you need to return the maximum profit that you can earn.
Lets say you decide that price of your app is Rs. x and there are N number of buyers. So maximum profit you can earn is :
 m * x
where m is total number of buyers whose budget is greater than or equal to x.

**Input format :**
```
Line 1 : N (No. of buyers)
Line 2 : Budget of buyers (separated by space)
```
**Output Format :**
```
Maximum profit
```

**Constraints :**
```
1 <= N <= 10^6
```
**Sample Input 1 :**
```
4
30 20 53 14
```
**Sample Output 1 :**
```
60
```
**Sample Output 1 Explanation :**
```
Price of your app should be Rs. 20 or Rs. 30. For both prices, you can get the profit Rs. 60.
```

**Sample Input 2 :**
```
5
34 78 90 15 67
```
**Sample Output 2 :**
```
201
```
**Sample Output 2 Explanation :** 
```
Price of your app should be Rs. 67. You can get the profit Rs. 201 (i.e. 3 * 67).
```

## Q4: Equal Sum Pair (Evaluate)

Given an integer array of size N, determine whether 4 elements exist such that a+b = c+d. Return true or false accordingly.
Perform this in O(n^2).
Note : (a+b) and (c+d) is unique. For eg, array(10, 10, 8, 9) Pair(10(at index 0),8) and Pair(10(at index 1),8) are different pairs but Pair(10(index 0),10(index 1)) and Pair(10(index 1),10(index0)) are same.
**Input Format :**
```
Integer N (size of input array)
```
**Output Format :**
```
true or false
```
**Contraints :**
```
1<= N <=10^3
```
**Sample Input 1:**
```
6
9 8 17 20 30 40
```
**Sample Output 1:**
```
false
```
**Sample Input 2:**
```
6
9 8 7 10 20 30
```
**Sample Output 2:**
```
true
```
**Sample Output 2 Explanation :**
```
9+8 = 10+7
Hence 4 elements exist which satisfy this relation.
```
**Sample Input 3:**
```
6
100 250 3 3 600
```
**Sample Output 3:**
```
true
```
**Sample Output 3 Explanation :**
```
100+3 (3 at index 1) = 100+3 (3 at index 2)
```

## Q5: Node having sum of children and node is max (Evaluate)

Given a tree, find and return the node for which sum of data of all children and the node itself is maximum. In the sum, data of node itself and data of immediate children is to be taken.

**Input format :**
```
Line 1 : Elements in level order form separated by space (as per done in class). Order is -

Root_data, n (No_Of_Child_Of_Root), n children, and so on for every element
```

**Output format :** 
```
Node with maximum sum.
```
**Sample Input 1 :**
```
5 3 1 2 3 1 15 2 4 5 1 6 0 0 0 0
```
**Sample Output 1 :**
```
1
```

## Q6: Make your Robot Smarter (Evaluate)

AI has provided bots to learn human skills but still they are very much limited as everything needs to be taught. You as a developer needs to write a robust framework using OOPs concepts that allows the users to add new skills to the Bot.

Provided below is the Interface of the Skill and Robot class that serves as an instance to the final bot. And add the following skills

1. WhatIsMyName
2. WhoCreatedYou
3. WhatSkillsYouHave

```
from abc import abstractmethod

class Robot:
    """
        Robot class 
    """
    def __init__(self):
        pass

    def ask(self, query):
        """
            Ask any query related to the skill, I will execute and print the answer
        """
        pass


class Skill: 
    """
        Skill Class
    """
    @abstractmethod
    def execute(self):
        pass
```


