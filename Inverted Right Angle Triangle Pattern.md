## 01. Inverted Right Angle Triangle Pattern

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/inverted-right-angletriangle-1605691171--104349/1)

### Problem Description

**Task:** Given an integer n, the task is to print an inverted right-angled triangle pattern using the * character. The pattern contains n rows, with the first row containing n stars and each subsequent row containing one fewer star.Examples: Input: n = 5

#### Examples

##### Example 1

- **Explanation:** Length of perpendicular and base of triangle is 3.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-22 20:28:18
- **Status:** Correct
- **Marks:** 2

```cpp
class Solution {
  public:
    void rightPattern(int n) {
        // code here
        for(int i=n;i>0;i--){
            for(int j=1;j<=i;j++){
                cout<<"*";
            }
            cout<<endl;
        }
    }
};
```

*Generated on: 11/22/2026, 8:32:55 PM*