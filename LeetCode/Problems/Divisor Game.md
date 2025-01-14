https://leetcode.com/problems/divisor-game/description/

- Problem : Alice and Bob play a game where given a number n, they have to give a number x , `1<x<n` and `n%x==0`. Then `n=n-x` and the other player takes the turn. If the other player cannot give a number, Alice wins and return True, else return False.
- Intuition : 
	- Base case : for n=1 -> False, n=2 -> True and n=3 -> False 
	- After base case : 
		- For any number n>3, ex n=4, we have 4=2x2 and 4=1x4. Therefore for n=4, moves are !(n=2) or !(n=1). Because we assume they play optimally, we choose the True value through 'or'
		- Similarly for any number n, if we find its appropriate factors' boolean value, we can memoize it to find the n value

- Code
```python

class Solution:

def divisorGame(self, n: int) -> bool:

checks=[False,True,False]

if n<=3:

return checks[n-1]

def findFac(v):

facs=[1]

for i in range(2,v):

if v%i==0:

facs.append(i)

facs.append(v//i)

return facs

for i in range(3,n):

checks.append(False)

for i in range(3,n):

facs=findFac(i+1)

for y in facs:

checks[i]=checks[i] or not checks[y]

print(checks)

return checks[n-1]
```
