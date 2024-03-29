### 冲突
冲突（collision）：给两个键分配的位置相同。

最简单的避免办法：如果两个键映射到同一个位置，就在这个位置存储一个链表。

假如所有键都被分配到同一个位置上，那么这就等同于将所有元素储存进一个链表里。这样的话查找速度会很慢。

### 教训
1. 散列函数很重要。前面的散列函数将所有的键都映射到一个位置，而最理想的状况下，散列函数均匀地将键映射到散列表的不同位置。
2. 如果散列表存储的链表很长，散列表的速度将极速下降。然而，如果使用的散列函数很好，这些链表就不会很长。