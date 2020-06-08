# SOLVING-TSP-FOR-METRIC-GRAPHS-USING-MST-HEURIST

# 1.1	Purpose 

The goal of this project is to build a program that solves Travelling salesman problem using optimal solution and compare it with the approximation solution.
# 1.2	The Problem Definition 

Travelling salesman problem (also called travelling salesperson problem or TSP) is an NP-hard problem in combinatorial optimization. TSP problem asks a question: given a list of cities and the distances between each pair of cities, what is the shortest route that visits each city and returns to the start city?  


# 1.3	Deep Explanation of The Problem

TSP have various solutions, but not all of them get the optimal solution. 
Exact Algorithms: are algorithms that always solve an optimization problem to optimality.
And we will try to solve the problem Using brute-force approach - it’s an Exact Algorithm - that will find the optimal solution, but it takes Θ(n!), which is impractical even for 20 cities.

Approximation Algorithms: are efficient algorithms that find approximate solutions to optimization problems in polynomial time.
Approximation algorithms are faster than the Exact algorithms. following its name, approximation algorithms cannot get the optimal solution always.
And we will try to solve the problem Using Christofide’s algorithm which gives at most 1.5 times the optimal.
Christofide’s algorithm works as the following:
For making an Eulerian graph, we have to find a minimum spanning tree and combine it with a minimum-weight perfect matching graph from the MST`s odd vertices.
So, now we can find the Eulerian tour since every vertex in the graph has even degree.
Finally, convert the Eulerian tour to TSP using shortcuts by removing the repeated vertices.

