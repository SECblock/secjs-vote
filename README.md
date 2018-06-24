# 这个库实现：

1. 当多个节点在工作周期内同时属于同一个自治域时，负责为这些节点进行投票，得票低者负责数据打包上链
投票的数据类型为Float，范围为1以内的8位小数

# 方法有：

```

1: getVoteNumber() // 为自己所在节点生成票数（随机的0-1的八位小数）

2: getNodeKey() // 为自己所在节点生成身份编号（四位整数代码）

3: getVote(nodeKey) // 获取目标节点的票数

4: getMinVoteNumber // 比对获得最小投票数

```