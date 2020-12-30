# 三对集(3DM)问题。

**实例:** 集合 $M \subseteq W \times X \times Y,$ 其中 $W 、 X 、 Y$ 是互不相交的集合, $\quad$ 且 $|W=| X|=| Y \mid=q$ 。

> $\times$ 表示笛卡尔积，表示两个集合中元素的所有组合可能，$\{1,2\} \times \{3,4\} = \{\{1,3\},\{1,4\},\{2,3\},\{2,4\}\}$, 在该问题中，$M$ 中的每一个元素是一个三元组，每个三元组的三个分量分别来自 $W,X,Y$


**询问:** $M$ 是否包含有一个完美对集(matching) $M^{\prime} \subseteq M,$ 使得 $|M^{\prime}|=q$ 且 $M^{\prime}$ 中没有任何 两个三元组有相同分量。 若 $M$ '是完美对集，则 $W 、 X 、 Y$ 中的每一个元素必出现在 $M^{\prime}$ 的一个且仅一个三元组中。

> 对 $W=\{1,2\},X=\{3,4\},Y=\{5,6\}$ 而言，若 $M=\{\{1,3,5\},\{2,4,6\},\{1,3,6\}\}$，那么 $M'$ 存在且 $M'=\{\{1,3,5\},\{2,4,6\}\}$ 是一个完美对集。
> 
> 若 $M=\{\{1,2,4\},\{2,4,6\},\{1,3,6\}\}$，那么该集合中就不存在完美对集，使得所有来自 $W,X,Y$ 中的元素仅出现一次。


# NPC 证明

**方法：**通过将 3DM 归约到 [3SAT](3sat.html) 问题来证明该问题属于 NPC

