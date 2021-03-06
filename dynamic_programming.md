### 有趣的事实：

BFS和PQ都是DP

* BFS是优先演绎

### 算法的本质

所谓的算法就是从⼀个起点状态，通过⼀系列空间和时间的运算，到达⼀个终点状态。⽤⼤⽩话说，我们就是在迷宫中从起点⾛向终点

* 备忘memo【从终点到起点】【孙老师讲的从右到左】
* 演绎【从起点到终点】【孙老师讲的从左到右】

### DP解题顺序

* 构建解空间\(树\)
* 计算节点值
* 计算edge的推导关系【一般是包含在节点值的计算当中】
* 寻找重复节点进行剪枝prune

### 解空间\(可视化\)树

* Node 当前状态的计算
* Edge 状态的推导

### 复杂度

我们在整条路上⾛的路径总⻓度就是我们的算法复杂度，⽽在⾛路过程中我们临时记录的数据的⼤⼩就是我们的空间复杂度。

* 时间复杂度
* * 总计算复杂度 = 节点个数 \* 每个节点的计算复杂度
* 空间复杂度
* * 栈的最深深度 \* 每个栈的空间复杂度 + 全局变量的空间复杂度
  * * 有的时候在判断是平方还是立方的颗粒度的时候取最大的就好

### 维度空间

* 1D，解空间的表示：F\(n\)，能够⽤⼀个变量表示解空间的⼀个节点。
* 2D，解空间的表示：F\(m, n\)，能够⽤两个变量表示解空间的⼀个节点。
* 3D，解空间的表示：F\(m, n, k \)，能够⽤三个变量表示解空间的⼀个节点。
* 比特空间，能够⽤⼀个bit表示⼀个元素是否存在，往往⽤来对⼀个维度进⾏深度建模。

> Leetcode上题目还是以1D和2D为主【占据了90%】

### **推导**

* 尾部拼接
* * Edge是和临近节点的推导得来
  * 孙老师说的『回头看一个』
* 选点拼接
* 确定一个点或者多个点
* * 孙老师说的『回头看多个，但是特点的点数』
* 区间拼接
* * 从i到j选择一个最优值
  * 如果跟终点没有关系，只和起点有关系，所以可以降为到和长度有关系
  * 孙老师说的『回头看多个，其实是回头看一个范围』

用孙老师的话来说：演绎是『回头看』，备忘是『往前看』

> Leetcode上题目的推导是以尾部拼接为主的，选点和区间次之



### 其他题目自己做

* 首先是想思路
* 如果很长时间内，思路想不到就不要浪费时间，开始看别人的思路【不要纠结是否最优解】
* 如果知道思路但是很长时间内做不出来，那就代表
* * 思路不清晰，更详细的更清楚的去理解思路
  * coding基本功差，多练习
* 关键是不要长时间的冥思苦想，大概10分钟为限



