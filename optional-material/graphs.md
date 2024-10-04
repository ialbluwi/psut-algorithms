## Shortest Paths

* Check [this video](https://www.youtube.com/watch?v=_Zhx4b3ygNg) to see how Dijkstra's algorithm is used/modified in practice to solve real-world problems like route finding.
* Check also [this video](https://youtu.be/bRvs8rOQU-Q?feature=shared&t=946), which compares Dijkstra's algorithm to the A* algorithm (you should see this algorithm in the AI course). The A* algorithm can be looked at as another way to speed-up Dijkstra's algorithm.
* Bellman-Ford's algorithm is a surprisingly-simple shortest paths algorithm that can handle negative edge weights. Here is a [long video](https://www.youtube.com/watch?v=ozsuci5pIso) explaining the algorithm (if you like proofs!) and a [shorter one](https://www.youtube.com/watch?v=9PHkk0UavIM), if you just want the gist of it!.

## Minimum Spanning Trees

While Prim's algorithm is probably the most widely used algorithm for finding minimum spanning trees, it is not the only one. Another famous and efficient algorithm is Kruskal's algorithm, which is worth learning about (this algorithm was covered in this course in previous semesters!). Here is a [long video](https://drive.google.com/file/d/1klMkfV-ozWPoFEMxnAkURyFjn61Xb8c5/view?usp=sharing) explaining the algorithm, its implementation and running time analysis. Here is also a [visualization](https://www.youtube.com/watch?v=vmWSnkBVvQ0) of the difference between Prim's and Kruskal's algorithms. If you are in a hurry, check this [much shorter video](https://www.youtube.com/watch?v=qOv8K-AJ7o0) (by Kruskal's cousin) explaining its main idea.

## Finding Strongly Connected Components

We covered what strongly connected components are but did not cover any algorithm for finding them! This problem is slightly harder than the problem of finding connected components in an undirected graph, which can be done with a single BFS or DFS as we have seen. Here is a [video](https://drive.google.com/file/d/148ldrDQVYXMiVSNX4s4zS84QfSjH0xvr/) explaining Kosaraju's algorithm (recorded at PSUT in Fall 2020). 
