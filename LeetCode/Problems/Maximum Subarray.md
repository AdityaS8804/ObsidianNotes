https://leetcode.com/problems/maximum-subarray/description/
- Problem : Given an array, find the sum of any subarray s.t. the sum is the maximum for the given array
- Intuition : 
	- Base case : `sums[0]` is `nums[0]`
		- After base case : `sums[i]=max(sums[i-1]+nums[i],nums[i])` . This chooses`sums[i]` s.t. the continuous subarray does not decrease the sum

- Code
```python
def maxSubarray(nums:list)->int:
	sums=[]
	sums[0]=nums[0]
	m=nums[0]
	for i in range(1,len(nums)):
		sums[i]=max(sums[i-1]+nums[i],nums[i])
		m=max(sums[i],m)
	return m
```
