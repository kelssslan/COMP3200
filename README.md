# Path Finder
Course: COMP 3200 Algorithmic Techniques for Artificial Intelligence
Topics: BFS, DFS, Greedy algorithm, heuristic functions
Professor:  **David Churchill https://www.cs.mun.ca/~dchurchill/**

A special thanks to Dr.Churchill for implementing a fun and great way to learn path searching methods. And also for giving me permission to share my experience with these assignments. Dr.Churchill spent months programming these assignments and the source codes are not available. Please sent me an email klan@mun.ca if you have any questions! 



![Screen Shot 2021-09-05 at 16 15 35](https://user-images.githubusercontent.com/66441548/132137983-255fa44b-e686-4216-9ea9-ee02158a82d5.png)



For this assignment, students were required to implement BFS, DFS methods to find the shortest path between two locations. The target can be of size 1x1, 2x2 or 3x3 grids. Heuristic functions were implemented to guess how much distance remaining. There were four different heuristics: Eucildean 2D distance, Cardinal Manhattan, Diagonal Manhattan, Return Zero.
The program must also pass random tests located at the left side.


![Screen Shot 2021-09-05 at 16 11 33](https://user-images.githubusercontent.com/66441548/132137881-999b0d61-6dbc-408d-8fc7-a1bedab03259.png)

Students were also required to test the connectivity of the path, meaning the 3x3 grid could only move in the grids that were in pink.

![Alt Text](https://github.com/kelssslan/PathFinder/blob/main/%20StudentA.gif)
![Alt Text](https://github.com/kelssslan/PathFinder/blob/main/StudentA1.gif)
![Alt Text](https://github.com/kelssslan/PathFinder/blob/main/StudentA2.gif)


The following GIFS above shows my code finding the shortest path on different maps.
**Red represents closed/already explored nodes
Yellow represents opened/exploring nodes**

![Alt Text](https://github.com/kelssslan/PathFinder/blob/main/WeightedA.gif)

The GIF above shows that we can tweak the performance of the path searcher by **adding a parameter weight w.**
Then multiply our heuristic results by w.
As we set the weight>1, then the path searcher favors going in the direction of the heuristic more and more
If the weight is <1, then the path searcher trusts the heuristic less and less.
