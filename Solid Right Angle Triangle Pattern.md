## 01. Solid Right Angle Triangle Pattern

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/right-angle-triangle-1605685807/1)

### Problem Description

**Task:** Given an integer n. Write a program to print the Right angle triangle wall. The length of perpendicular and base is s. Note: Print exactly single " " after "*". Print a new line after printing the triangle.Examples:Input: n = 4

#### Examples

##### Example 1

- **Explanation:** * * * * * * * * * * Explanation: Length of perpendicular and base of triangle is 4 .Input: n = 3 * * * * * * Explanation: Length of perpendicular and base of triangle is 3.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-22 19:49:53
- **Status:** Correct
- **Marks:** 2

```cpp
class Solution {
  public:
    void printPattern(int n) {
        // code here
        for(int i=0;i<n;i++){
           for(int j=0;j<=i;j++){
               cout<<"* ";
           } 
           cout<<endl;
        }
        
    }
};
```

*Generated on: 11/22/2026, 7:50:20 PM*