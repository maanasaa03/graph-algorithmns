# graph-algorithmns

prims:
it gives a mst of cost 8. but this cost can be reduced to 1 if the negative edge between d and e is taken into consideration.

kruskals:
the mst returned is not connected.

this is because prims and kruskals donot work for directed graphs.
in prims,it assummes all nodes are connected which is not true for directed graphs.
in kruskals,there can be cases where there is no cycle in the directed graoh but the algorithm considers it to exist since there is a connection between the nodes.

djikstras:
the shortest path from a to d is given with cost 5. but this can be reduced to cost 2 if the negative edge is taken into consideration.
This is because Dijkstra’s algorithm believes that all costs in the given graph are non-negative, so adding any positive number on a vertex that has already been visited will never change its minimality. this problem can be solved by using bellman ford algorithm instead.

I have used C since it is the programming language i am most familiar with.
