## 01. Last Coin in Game of Alternates

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/last-coin-in-a-game-of-alternates/1)

### Problem Description

**Task:** Given an array integer arr[] , representing the values of coins arranged in a row.Two players play a game by picking coins alternately.At each turn, a player can pick a coin from either the beginning or the end of the array. Both players follow a greedy strategy, i.e., they always pick the coin with the maximum value among the two available ends.The game continues until only one coin remains.Find the value of the last remaining coin.Examples:Input : arr[] = [5, 3, 1, 6, 9]

#### Examples

##### Example 1

- **Output:**
```text
11Explanation:Only one coin is present in the array, so no moves are made. Final Output: 11
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-15 18:41:23
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    int coin(vector<int>& arr) {
        // code here
        int i=0;
        int j=arr.size()-1;
        
        while(i<j){
            if(arr[i]>arr[j]){
                i++;
            }
            else{
               j--; 
            }
        }
        return arr[i];
        }
    };
```

*Generated on: 11/15/2026, 6:41:52 PM*