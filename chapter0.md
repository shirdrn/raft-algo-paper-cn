## 摘要

`Raft` 是一种用来管理日志复制的一致性算法。它产生的结果等价于 `Paxos` ，而且同样有效，但是它的结构不同于 `Paxos`；这使得 `Raft` 比`Paxos` 更易于理解，并为建立实际的系统提供了更好的基础。为了增强可理解性，`Raft` 可分为三个关键的一致性元素，例如`Leader`选举（`Leader Selection`）、日志复制（`Log Replication`）和安全（`Safety`），并且它通过减少需要考虑的状态数，来强制加强一致性的度量。通过用户学习的结果表明，`Raft` 比 `Paxos` 更容易学习。`Raft` 还包括了一种动态改变集群成员的新机制，它使用重叠大多数（`Overlapping Majorities`）的方式来保证安全。

