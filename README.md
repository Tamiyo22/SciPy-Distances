# SciPy-Distances
Euclidean Distance .euclidean()
Manhattan Distance .cityblock()
Hamming Distance .hamming()
There are a few noteworthy details to talk about:

First, the scipy implementation of Manhattan distance is called cityblock(). Remember, computing Manhattan distance is like asking how many blocks away you are from a point.

Second, the scipy implementation of Hamming distance will always return a number between 0 an 1. Rather than summing the number of differences in dimensions, this implementation sums those differences and then divides by the total number of dimensions. For example, in your implementation, the Hamming distance between [1, 2, 3] and [7, 2, -10] would be 2. In scipy‘s version, it would be 2/3.

