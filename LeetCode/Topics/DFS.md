- Methodology
	- Using recursion -> call dfs function for each node in 'neighbors' list
		- Think about what the 'neighbors' are as per the problem
	- In graphs, issue is with cycles. Therefore, always have if...else or boolean array to check if the node is already visited, eg: if node has been already cloned
	- In matrices, to prevent re-counting, change the initial value to something else
- Extra Points 
	- Think of combining BFS and DFS as needed.
	- 

- Problems
	1. [[133. Clone Graph]] 
	2. [[934. Shortest Bridge]]