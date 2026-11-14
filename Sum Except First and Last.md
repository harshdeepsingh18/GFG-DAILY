## 01. Sum Except First and Last

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/max-length-chain/1)

### Problem Description

**Task:** Given an array arr of numbers. Return the sum of all the elements except the first and last elements.Examples:Input: arr[] = [5, 24, 39, 60, 15, 28, 27, 40, 50, 90]

#### Examples

##### Example 1

- **Output:**
```text
283
```
- **Explanation:** The sum of all the elements except the first and last element is 283.

##### Example 2

- **Input:**
```text
arr[] = [5, 10, 1, 11]
```
- **Output:**
```text
11
```
- **Explanation:** The sum of all the elements except the first and last element is 11.

##### Example 3

- **Input:**
```text
arr[] = [5, 10]
```
- **Output:**
```text
0
```
- **Explanation:** The sum of all the elements except the first and last element is 0.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (C++)

- **Submitted:** 2026-11-14 21:41:10
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution {
  public:
    int sumExceptFirstLast(vector<int>& arr) {
        // code here{
        int sum=0;
        for(int i=1;i<arr.size()-1;i++){
            sum=sum+arr[i];
        }
        return sum;
    }
};
```

#### Solution 2 (C++)

- **Submitted:** 2026-11-14 21:40:57
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    int sumExceptFirstLast(vector<int>& arr) {
        // code here{
        int sum=0;
        for(int i=1;i<arr.size()-1;i++){
            sum=sum+arr[i];
        }
        return sum;
    }
};
```

*Generated on: 11/14/2026, 9:41:36 PM*