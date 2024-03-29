##  最长公共子串
### 启示
1. 动态规划可帮助你在给定约束条件下找到最优解。在背包问题中，你必须在背包容量给定的情况下，偷到价值最高的商品。
2. 在问题可分解为彼此独立且离散的子问题时，就可使用动态规划来解决。

### 设计动态解决方案的要点
* 每种动态规划解决方案都涉及网格。
* 单元格中的值通常就是你要优化的值。在前面的背包问题中，单元格的值为商品的价值。
* 每个单元格都是一个子问题，因此你应考虑如何将问题分成子问题，这有助于你找出网格的坐标轴。

例：

Alex在查找词典时输入了hish，那他原本要输入的是fish还是vista呢？

### 绘制网格

* 单元格中的值是什么？
* 如何将这个问题划分为子问题？
* 网格的坐标轴是什么？

在动态规划中，要将某个指标最大化。在这个例子中，要找出两个单词的最长公共子串。hish 和 fish 都包含的最长公共子串是什么？ hish 和 vista 呢？