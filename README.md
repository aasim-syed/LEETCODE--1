# LEETCODE--1

### Palindrome Number
```
9. Palindrome Number
Easy

4661

1952

Add to List

Share
Given an integer x, return true if x is palindrome integer.

An integer is a palindrome when it reads the same backward as forward.

For example, 121 is a palindrome while 123 is not.
 

Example 1:

Input: x = 121
Output: true
Explanation: 121 reads as 121 from left to right and from right to left.
Example 2:

Input: x = -121
Output: false
Explanation: From left to right, it reads -121. From right to left, it becomes 121-. Therefore it is not a palindrome.
Example 3:

Input: x = 10
Output: false
Explanation: Reads 01 from right to left. Therefore it is not a palindrome.
 

Constraints:

-231 <= x <= 231 - 1
<comment>

<h2>JAVA-CODE</h2>
```
<hr>
```

 class Solution {
    public boolean isPalindrome(int x) {
       int rev = 0;
        int x1 = x;
        if(x<0){
            return false;
        }
        while(x != 0)
        {
        
        int d = x % 10;
        rev = rev * 10 + d;
        x /= 10;
                           }
        return (rev == x1);
        }
}
```             

![image](https://user-images.githubusercontent.com/70385414/147397641-3697f564-094a-498a-ab99-c307f3bfe3f8.png)
