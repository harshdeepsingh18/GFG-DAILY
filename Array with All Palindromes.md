## 01. Array with All Palindromes

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/palindromic-array-1587115620/1)

### Problem Description

**Task:** Given an array arr[] of positive integers. Return true if all the array elements are palindrome otherwise, return false.Examples:Input: arr[] = [111, 222, 333, 444, 555]

#### Examples

##### Example 1

- **Output:**
```text
false
```
- **Explanation:** 20 is not a palindrome hence the output is false.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-14 13:39:47
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
public:
    bool isPalinArray(vector<int> &arr) {
        // code here
        for(int i = 0; i < arr.size(); i++) {

            int num = arr[i];
            int original = num;
            int reverse = 0;

            while(num > 0) {
                int digit = num % 10;
                reverse = reverse * 10 + digit;
                num = num / 10;
            }

            if(original != reverse) {
                return false;
            }
        }

        return true;
    }
};
```

*Generated on: 11/14/2026, 1:40:14 PM*