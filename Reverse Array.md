## 01. Reverse Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/reverse-an-array/1?utm_source=chatgpt.com)

### Problem Description

**Task:** Given an array of integers arr[], reverse the array in place.Examples:Input: arr = [1, 4, 3, 2, 6, 5]

#### Examples

##### Example 1

- **Output:**
```text
[1]Explanation: The array has only single element, hence the reversed array is same as the original.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-14 11:14:05
- **Status:** Correct
- **Marks:** 2

```cpp
class Solution {
  public:
    void reverseArray(vector<int> &arr) {
        // code here
        int n=arr.size();
        int i=0;
        int j=n-1;
        while(i<j){
            swap(arr[i],arr[j]);
            i++;
            j--;
        
        }
    }
};
```

*Generated on: 11/14/2026, 11:14:35 AM*