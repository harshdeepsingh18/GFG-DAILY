## 01. Palindrome Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/perfect-arrays4645/1)

### Problem Description

**Task:** Given an array arr[], the task is to find whether the arr is palindrome or not. An array is said to be palindrome if its reverse array matches the original array.

#### Examples

##### Example 1

- **Input:**
```text
arr = [1, 2, 3, 2, 1]
```
- **Output:**
```text
true
```
- **Explanation:** If we reverse, we get [1, 2, 3, 2, 1] which is the same as before. So, the answer is true.

##### Example 2

- **Input:**
```text
arr = [1, 2, 3, 4, 5]
```
- **Output:**
```text
falseExplanation: If we reverse it, we get [5, 4, 3, 2, 1] which is the not same as before. So, the answer false.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-14 22:26:28
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    bool isPalindrome(vector<int> &arr) {
        // code here
       int i=0;
       int j=arr.size()-1;
       while(i<j){
           if(arr[i]!=arr[j]){
               return false;
               
               
           }
         i++;
         j--;
        
           
       }
    return true;
    }
};
```

*Generated on: 11/14/2026, 10:29:53 PM*