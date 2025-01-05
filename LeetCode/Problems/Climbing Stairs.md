https://leetcode.com/problems/climbing-stairs/description/

- Problem : Given a number of stair, n, it can be climbed only in increments of 1 or 2. Find the total number of possible ways to climb n number of stairs
- Intuition : 
	- Base case : 1 stair - 1way; 2 stairs - 1+1,2 - 2 ways; 3 stairs - 1+1+1,1+2,2+1 - 3ways
	- After base case : 
		- For climbing 4 stairs - climb 3 stairs and one more stair + climb 2 stair and 2 more stairs. 
		- Therefore for climbing n stairs, no. of ways to climb n-1 stairs + number of ways to climb n-2 ways

- Code
```python
def climbStairs(n:int)->int:
	if n<=3:
		return n
	prev2=3
	prev1=2
	curr=0
	for _ in range(3,n):
		curr=prev2+prev1
		prev1=prev2
		prev2=curr
	return curr
	
```
