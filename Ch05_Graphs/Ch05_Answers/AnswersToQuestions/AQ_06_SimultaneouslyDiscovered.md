﻿5-6. In breadth-first and depth-first search, an undiscovered node is marked discovered when it is first encountered, and marked processed when it has been completely searched. At any given moment, several nodes might be simultaneously in the discovered state. 

(a) Describe a graph on n vertices and a particular starting vertex v such that Θ(n) nodes are simultaneously in the discovered state during a breadth-first search starting from v. 

(b) Describe a graph on n vertices and a particular starting vertex v such that Θ(n) nodes are simultaneously in the discovered state during a depth-first search starting from v. 

(c) Describe a graph on n vertices and a particular starting vertex v such that at some point Θ(n) nodes remain undiscovered, while Θ(n) nodes have been processed during a depth-first search starting from v. (Note, there may also be discovered nodes.)


<details>
<summary>**ANSWER**</summary>
  <p>

(a) A graph with root v and depth 1 (all n nodes are directly accessible from the root v).

(b) A graph with root v and a linear chain of n nodes.

(c) A graph with root v and two equal linear branches of lengths n/2.

  </p>
</details>