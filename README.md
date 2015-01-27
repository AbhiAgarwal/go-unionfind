# Union Find

A quick implementation of Union-Find in Go. 

- A union–find algorithm is an algorithm that performs two useful operations on such a data structure
	- Find: Determine which subset a particular element is in. This can be used for determining if two elements are in the same subset
	- Union: Join two subsets into a single subset
- Bound
	- O(nlog(n))
- Uses
	- Disjoint-set data structures model the partitioning of a set, for example to keep track of the connected components of an undirected graph.
	- This model can then be used to determine whether two vertices belong to the same component, or whether adding an edge between them would result in a cycle.
	- The Union–Find algorithm is used in high-performance implementations of unification.

Simple Program

```
go get github.com/AbhiAgarwal/go-unionfind
```

```go
package main

import (
	"fmt"
	unionfind "github.com/AbhiAgarwal/go-unionfind"
)

func main(){
	union := unionfind.NewUnionFind()
	union.UnionFind(4)
	fmt.Println(union.NumSets)
}
```