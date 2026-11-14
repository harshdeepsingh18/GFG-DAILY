## 01. Count Smaller in Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/count-of-smaller-elements5947/1)

### Problem Description

**Task:** Given an unsorted array arr[]. Find the count of elements less than or equal to the given element x.Examples:Input: x = 9, arr[] = [10, 1, 2, 8, 4, 5]

#### Examples

##### Example 1

- **Output:**
```text
4 Explanation: The 4 elements are 1, 2, 2 and 2.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-14 14:19:21
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    int countOfElements(int x, vector<int> &arr) {
        // code here
        int count=0;
        for(int i=0;i<arr.size();i++){
            if(arr[i]<=x){
                count++;
            }
            
        }
        return count;
    }
};
```

*Generated on: 11/14/2026, 2:19:48 PM*