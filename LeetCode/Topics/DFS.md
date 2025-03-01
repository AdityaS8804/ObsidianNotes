- Methodology
	- Using recursion -> call dfs function for each node in 'neighbors' list
		- Think about what the 'neighbors' are as per the problem
	- In graphs, issue is with cycles. Therefore, always have if...else or boolean array to check if the node is already visited, eg: if node has been already cloned
	- In matrices, to prevent re-counting, change the initial value to something else
- Extra Points 
	- Think of combining BFS and DFS as needed.
	- When given DAG - need not check for repetitions -> no cycles so no repetitions can occur

- Problems
	1. [[133. Clone Graph]] 
	2. [[934. Shortest Bridge]]
	3. [[130. Surrounded Regions]]
	4. [[797. All Paths From Source to Target]]
	