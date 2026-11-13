## 01. Min and Max in Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/find-minimum-and-maximum-element-in-an-array4428/1)

### Problem Description

**Task:** Given an array arr[]. Your task is to find the minimum and maximum elements in the array.Examples:Input: arr[] = [1, 4, 3, 5, 8, 6]

#### Examples

##### Example 1

- **Output:**
```text
[3, 15]Explanation: minimum and maximum element of array are 3 and 15.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (3)

#### Solution 1 (C++)

- **Submitted:** 2026-11-13 21:17:55
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution {
  public:
    vector<int> getMinMax(vector<int> &arr) {
        // code here
        int mn=INT_MAX;
        int mx=INT_MIN;
           
        for(int i=0;i<arr.size();i++){
            mn=min(arr[i],mn);
            mx=max(arr[i],mx);
            
            
        }
        return {mn,mx};
    }
};
```

#### Solution 2 (C++)

- **Submitted:** 2026-11-13 09:55:30
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution {
    public ArrayList<Integer> getMinMax(int[] arr) {
        // code Here
       int min = arr[0];
              int max = arr[0];

              for (int i = 1; i < arr.length; i++) {

                  if (arr[i] < min) {
                      min = arr[i];
                  }

                  if (arr[i] > max) {
                      max = arr[i];
                  }
              }

              ArrayList<Integer> result = new ArrayList<>();
              result.add(min);
              result.add(max);

              return result;
       }
}
```

#### Solution 3 (C++)

- **Submitted:** 2026-11-13 09:55:24
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
    public ArrayList<Integer> getMinMax(int[] arr) {
        // code Here
       int min = arr[0];
              int max = arr[0];

              for (int i = 1; i < arr.length; i++) {

                  if (arr[i] < min) {
                      min = arr[i];
                  }

                  if (arr[i] > max) {
                      max = arr[i];
                  }
              }

              ArrayList<Integer> result = new ArrayList<>();
              result.add(min);
              result.add(max);

              return result;
       }
}
```

*Generated on: 11/13/2026, 9:47:55 PM*