## 01. Elements in Range

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/elements-in-the-range2834/1)

### Problem Description

**Task:** Given an array arr[] containing distinct positive integers, and two integers start and end defining a range. Find if the array contains all elements within inclusive range [start, end].Examples :Input: start = 2, end = 5, arr[] = [1, 4, 5, 2, 7, 8, 3]

#### Examples

##### Example 1

- **Output:**
```text
false
```
- **Explanation:** The array does not contain 6; hence, it does not contain all the elements in the range [2, 6]. Therefore, the output is false.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-14 21:58:58
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    bool checkElements(int start, int end, vector<int> &arr) {
        // code here
        vector<int> ans;
        for(int i=0;i<arr.size();i++){
            if(arr[i]>=start && arr[i]<=end){
                ans.push_back(arr[i]);
            }
        }
        if(ans.size()==end-start+1){
            return true;
        }
        return false;
    }
};
```

*Generated on: 11/14/2026, 9:59:38 PM*