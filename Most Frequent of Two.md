## 01. Most Frequent of Two

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/who-has-the-majority/1)

### Problem Description

**Task:** Given an array arr[] and two elements x and y, return the element that occurs more frequently. If both elements have the same frequency, return the smaller one.

#### Examples

##### Example 1

- **Input:**
```text
arr[] = [1, 1, 2, 2, 3, 3, 4, 4, 4, 4, 5], x = 4, y = 5Output: 4
```
- **Explanation:** frequency of 4 is 4.frequency of 5 is 1.Since 4 > 1 so return 4

##### Example 2

- **Input:**
```text
arr[] = [1, 2, 3, 4, 5, 6, 7, 8], x = 1, y = 7
```
- **Output:**
```text
1
```
- **Explanation:** frequency of 1 is 1.frequency of 7 is 1.Since 1 < 7, return 1.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-14 21:35:46
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    int moreFrequent(vector<int>& arr, int x, int y) {
        // code here
        int Xcount=0;
        int Ycount=0;
        for(int i=0;i<arr.size();i++){
            if(arr[i]==x){
                Xcount++;
            }
        }
        
        for(int i=0;i<arr.size();i++){
            if(arr[i]==y){
                Ycount++;
            }
            
        }
        if(Xcount>Ycount){
            return x;
        }
        else if(Ycount>Xcount){
            return y;
        }
        else{
            return min(x,y);
        }
        
    }
};
```

*Generated on: 11/14/2026, 9:37:02 PM*