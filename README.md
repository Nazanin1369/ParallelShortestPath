## ParallelShortestPath

Parallel implementation of a shortest path algorithm


### What is it about?
The Shortest Path Faster Algorithm (SPFA) is an improvement of the Bellman–Ford algorithm which computes single-source shortest paths in a weighted directed graph. The algorithm is believed to work well on random sparse graphs and is particularly suitable for graphs that contain negative-weight edges. However, the worst-case complexity of SPFA is the same as that of Bellman–Ford, so for graphs with nonnegative edge weights Dijkstra's algorithm is preferred.[2] The SPFA algorithm was published in 1994 by Fanding Duan.

### Why parallel?
Since I have to compute the shortest path trees with origins in all nodes, it is only natural to do it in parallel (as the trees are independent of each other).

### How??
I'm doing it with the use of a pool of workers using the multiprocessing and appending the results to a list 

### How to run??
   javac *.java
   java Application
