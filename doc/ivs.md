# 独立集问题（Idpendent Vertice Set，IVS）

[独立集](./../GraphTheory/3.html)问题可以形式化表示为：

**实例：** 图 $G=(V,E)$，正整数$K$，

**询问：** 是否存在 $V$ 的子集$V'$，满足任意两点 $u,v\in V'$，$(u,v)\not\in E$，$|V'|>=K$。


该问题可以通过由 [顶点覆盖问题](./vc.html) 归约证明


## NPC 证明

如果一个图 $G=(V,E)$ 存在一个顶点覆盖 $|V'|<=L$，那么就存在一个独立集 $|V''|>=|V|-L$ 。

因为按照顶点覆盖的定义，其覆盖集 $|V'|$ 中的所有点，都有一条边与其相连，那么将 |V'| 从图 G 中删去时，图中就不再存在任何边，那么剩下的点自然就成为了独立集（也即任意两点之间不存在边）。

> 也可以得出， 顶点覆盖集+独立集=全部点集

构造独立集问题实例，只需要在顶点覆盖问题实例的基础上，令 $|V'|>=|V|-L$ 即可。

