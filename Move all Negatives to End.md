## 01. Move all Negatives to End

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/move-all-negative-elements-to-end1813/1)

### Problem Description

**Task:** Given an unsorted array arr[ ] having both negative and positive integers. Place all negative elements at the end of the array without changing the order of positive elements and negative elements.Note: Don't return any array, just in-place on the array.Examples:Input : arr[] = [1, -1, 3, 2, -7, -5, 11, 6 ]

#### Examples

##### Example 1

- **Output:**
```text
[7, 9, 10, 11, -5, -3, -4, -1]
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-15 14:07:14
- **Status:** Correct
- **Marks:** 2

```cpp
class Solution {
  public:
    void segregateElements(vector<int>& arr) {
        // code here
        vector<int> ans(arr.size());
        int j=0;
        for(int i=0;i<arr.size();i++){
            if(arr[i]>=0){
                ans[j]=arr[i];
                j++;
            }
        }
        for(int i = 0; i < arr.size(); i++) {
                    if(arr[i] < 0) {
                        ans[j]=arr[i];
                         j++;
                    }
                    
        }        
        for(int i=0;i<arr.size();i++){
            arr[i]=ans[i];
        }
    }
};
```

*Generated on: 11/15/2026, 2:07:44 PM*