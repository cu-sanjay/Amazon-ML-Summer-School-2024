<div align="center">
<h1> Programming Questions </h1>

## Question 1: Nearest Friend's House
</div>

You are given an array of integers **A** of size **N**. Each element in the array is distinct and represents the location of a friend's house as an x coordinate (i.e., if the array **A = [1,3,8]**, it means that there are 3 friends living at **x = 1, x = 3** and **x = 8**. It can be assumed that the array is sorted in ascending order.

The capacity of every friend's house is **N-1** (i.e., not more than **N-1** people can be there in the house together). Every friend wants to call **N-2** friends to their home (1 himself and **N-2** friends so that the total number of people in the house is **N-2**, i.e., the maximum capacity of the house).

Now they are in a dilemma as everyone has to decide which **N-2** friends to call. They come up with the strategy that they will call **N-2** friends such that the summation of the distances travelled by all the friends is the minimum.

For every **i**<sup>th</sup> friend, you need to return the minimum distance travelled by the **N-2** friends if they decide to meet at the **i**<sup>th</sup> friend's house.

**Input Specification:**
- `input1`: An integer value **N**
- `input2`: An integer array **A**

**Output Specification:**
- Return an array where each element represents the minimum distance travelled for the **ith** friend's house.

**Example:**

**Input:**
```
N = 5
A = [1, 2, 3, 4, 5]
```

**Output:**
```
[6, 4, 4, 4, 6]
```

## Explanation:
- The 1st friend's house is at **x = 1** and he has to call just 3 friends so it is better to call only the friends at **x = 2, x = 3,** and **x = 4**. So, the total distance travelled is **(2-1) + (3-1) + (4-1) = 6**.
- The 2nd friend's house is at **x = 2** and he has to call just 3 friends so it is better to call only the friends at **x = 1, x = 3,** and **x = 4**. So, the total distance travelled is **(2-1) + (3-2) + (4-2) = 4**.
- The 3rd friend's house is at **x = 3** and he has to call just 3 friends so it is better to call only the friends at **x = 1, x = 2,** and **x = 4**. So, the total distance travelled is **(3-1) + (3-2) + (4-3) = 4**.
- The 4th friend's house is at **x = 4** and he has to call just 3 friends so it is better to call only the friends at **x = 2, x = 3,** and **x = 5**. So, the total distance travelled is **(4-2) + (4-3) + (5-4) = 4**.
- The 5th friend's house is at **x = 5** and he has to call just 3 friends so it is better to call only the friends at **x = 2, x = 3,** and **x = 4**. So, the total distance travelled is **(5-2) + (5-3) + (5-4) = 6**.

So, the array **[6, 4, 4, 4, 6]** will be returned as the answer.

<div align="center">
<h2> Question 2: Pair Problem </h2>
</div>
Lucy has an integer array **A** of size **N**. All the elements in the array are distinct. She can perform the following operation any number of times:

- Choose two numbers **i** and **j** in such a way that the product of the LCM (**i, j**) and HCF (**i, j**) is present in array **A**.

Your task is to help Lucy find and return an integer value, representing the maximum number of valid **(i, j)** pairs which satisfy the given condition.

**Note:**
- The Least Common Multiple (LCM) of two numbers is the smallest number which is a multiple of both.
- The Highest Common Factor (HCF) is the greatest number which divides each of the two or more numbers.
- The pair of **(X, Y)** is different from the pair of **(Y, X)**

**Input Specification:**
- `input1`: An integer value **N**
- `input2`: An integer array **A**

**Output Specification:**
- Return an integer value, representing the maximum number of valid (ij) pairs which satisfy the given condition.

**Example:**

**Input:**
```
N = 5
A = {1, 2, 3, 4, 5}
```

**Output:**
```
10
```
