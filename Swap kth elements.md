## 01. Swap kth elements

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/swap-kth-elements5500/1)

### Problem Description

**Task:** Given an array arr[], swap the k^th element from the beginning with the k^th element from the end.Note: 1-based indexing is followed.Examples :Input: arr[] = [1, 2, 3, 4, 5, 6, 7, 8], k = 3

#### Examples

##### Example 1

- **Output:**
```text
[5, 1, 6, 3, 2]
```
- **Explanation:** 2^nd element from beginning is 3 and from end is 1.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-15 18:25:04
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    void swapKth(vector<int> &arr, int k) {
        // code here
        int n=arr.size();
        
        int first=k-1;
        int last=n-k;
        swap(arr[first],arr[last]);
        
    }
};
```

*Generated on: 11/15/2026, 6:25:33 PM*