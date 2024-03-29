### 使用狄克斯特拉算法（Dijkstra's algorithm）
![加权有向图](加权有向图.png)

其中每个数字表示的都是时间，单位分钟。为找出从起点到终点耗时最短的路径，你将使用狄克斯特拉算法。

如果使用广度优先搜索，那么找到的路径是：

* 起点→A→终点
* 起点→B→终点

这两种都是 7分钟。那么狄克斯特拉算法的计算结果如何呢？步骤如下：

1. 找出“最便宜”的节点，即可以在最短时间内到达的节点。
2. 对于该节点的邻居，检查是否有前往它们的更短路径，如果有，就更新其开销。
3. 重复这个过程，直到对图中每个节点都执行此操作。
4. 计算最终路径。

* 起点最邻近的是 B，两分钟；
* B最邻近的是 A，三分钟；
* A最邻近的是终点，一分钟；
* 起点→B→A→终点，这种路径只需要 6分钟；
* 重复以上步骤，更新 A节点所有的邻居开销；
* 没有比上面这条路径更快的，结束。
