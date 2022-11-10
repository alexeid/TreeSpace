# TreeSpace

## Ranked trees

A ranked tree is a rooted phylogenetic topology where every node is given a rank. For 
samples contemporaneous samples, all leaves have the same rank (0). The most recent 
internal node has rank 1 (necessarily a cherry), the next most recent internal node in the 
tree has rank (2) et cetera. The root will have rank $n-1$, where $n$ is the number of
taxa/leaves.

For 4 taxa this definition implies that there are 18 distinct ranked trees that could
describe the ancestral relationships of the taxa.

These 18 objects are the discrete component of the space of all trees for standard models 
of phylogeny, including coalescent and birth-death models of phylogenetic trees.

## Ranked NNI tree space

In addition to being able to enumerate all valid phylogenetic trees for a given number of
taxa, it may also be interesting to measure how similar two trees are. Once a 
neighbourhood function is defined for all trees then the distance between two trees 
can be defined as the shortest path via neighbours starting from one tree and ending at 
the other.

The ranked NNI tree space defines a neighbourhood of a phylogenetic tree to be all trees
that can be reached by one nearest-neighbour interchange (NNI) operation, or by one rank
move. In Figure 1 the 18 ranked trees on 4 taxa are depicted at nodes in a graph, with
edges connecting neighbouring trees. Straight edges change the unranked topology, while 
wavy edges change only the ranks of the nodes (a rank move).

<img src="images/treeSpace4-00.jpg?raw=true" width="600">

All of the edges in this graph represent the same distance (1) in ranked NNI tree space. 
The edges have different lengths in this depiction of the space because the graph is being
visualised in the two-dimensional plane. This projection causes distortions. 

The next figure highlights the "shells" of nodes that are 0 (yellow), 1 (orange), 2 (red) steps away from a focal 
tree coloured yellow. White trees are the maximum distance away (which is 3 steps for 4 
taxa).

<img src="images/treeSpace4-combTreeNeighbourhood-00.jpg?raw=true" width="600">
