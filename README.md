# java-maze
Java Maze assignment completed in April 2021 for Fundamentals of Computer Science II at Northeastern University. Unfortunately the code is available by request only due to the confidentiality rules at Northeastern University, this protects my work from plagarism by future students taking the course.

## Pair Programming
This assignments was programmed using the [Agile development](https://en.wikipedia.org/wiki/Agile_software_development) concept of [pair programming](https://en.wikipedia.org/wiki/Pair_programming). Pair programming has been proven to make cleaner code with less bugs than individual programming.

## Unit Testing
My partner and I wrote unit tests before we wrote code which reduced the overall number of bugs in our code. We used a testing library built at Northeastern University, `tester.jar`. This library is not as full featured as other software like JUnit and the complexity of this program pushed the library to it's limit.

## Graphs
The maze in this program is represented as an undirected graph. Each `Node` represents a node on the graph and each `Edge` is a vertex. The maze has a "wall" if the adjacent node is at a depth greater than 1. 

## Graph Traversal
Graph traversal is achieved using both depth-first and and breadth-first search algorithms by typing the `d` and `b` key respectively. 

### Depth-First Search
Depth first search is implemented using a `Queue` data structure. Nodes are added to the queue and then popped off in a first in first out (FIFO) order.

### Breadth-First Search
Breadth-first search is implementing using a `Stack` data structure. Nodes are added to the stack and then popped off in a last in first out (LIFO) order. 

## Maze Generation
The maze is a minimum spanning tree that is initialized using [Kruskal's Algorithm](https://en.wikipedia.org/wiki/Kruskal%27s_algorithm). The weights of the edges are set randomly so the maze is different each time the project is run. 

## Further Development
5 dreams I have if I were to develop this further:
1. Switch from the Northeastern Tester Library to the JUnit Testing Framework
   1. I Learned how to use JUnit in `Object Oriented Design` and will switch this project to use it eventually
2. Add access modifiers to all variables
   1. When I originally wrote this project I was new to Java syntax and Object Oriented concepts so I had no idea what access modifiers even were. Now I am wiser and know that these are essential for safe extensible code. 
3. Add more documentation
   1. The documentation is written using comments which makes them difficult to read and nearly impossible to find. 
4. Rename variables to be more descriptive
   1. Variables like `i`, `r`, and `k` take a long time to decipher after walking away from the code for a while.
5. Look into using a different framework like the `Swing Library`
