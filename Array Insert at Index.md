## 01. Array Insert at Index

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/array-insert-at-index/1)

### Problem Description

**Task:** Given an array arr(0-based index) and two positive integer index and val. You need to insert an val at given index.Examples:Input: arr[] = [1, 2, 3, 4, 5], index = 5, val = 90Output: 1 2 3 4 5 90

#### Examples

##### Example 1

- **Output:**
```text
[1, 2, 90, 3, 4, 5]
```
- **Explanation:** 90 is inserted at index 2(0-based indexing). After inserting, array elements are like [1, 2, 90, 3, 4, 5].

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-14 21:22:33
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    void insertAtIndex(vector<int> &arr, int index, int val) {
        // code here
        arr.push_back(0);
        for(int i=arr.size()-1;i>index;i--){
            arr[i]=arr[i-1];
        }
        arr[index]=val;
    }
};
```

*Generated on: 11/14/2026, 9:23:03 PM*