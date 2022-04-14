# big
```text
开源大数据技术学习期间产出
```
大数据特点：4V（大量、高速、多样、低价值密度）

# 第一章 Hadoop
## 1.1 Hadoop 入门
### 1.1.1 概念
#### 1、 Hadoop 是什么
```text
1) 分布式系统基础架构
2）主要解决，海量数据的存储和海量数据的分析计算问题
3）广义 ———— Hadoop 生态圈
```
#### 2、 Hadoop 发展历史
#### 3、 Hadoop 的三大发行版本
#### 4、 Hadoop 的优势（ 4 高）
```text
1）高可靠性：底层维护多个数据副本
2）高扩展性：在集群间分配任务数据，可方便的扩展数以千计的节点
3）高效性：并行工作
4）高容错性：能够自动将失败的任务重新分配
```
#### 5、 Hadoop 的组成
```text
1）Hadoop 1.x组成
    Common（辅助工具）
    HDFS（数据存储）
    MapReduce（计算 + 资源调度）
2）Hadoop 2.x组成
    Common（辅助工具）
    HDFS（数据存储）
    MapReduce（计算）
    Yarn（资源调度）
3）Hadoop 3.x组成（组成上没有变化）


* HDFS：分布式文件系统
    1）NameNode（NN）：存储文件的元数据，如文件名，文件目录结构，文件属性（生产时间、副本数、文件权限），以及每个文件的块列表和块所在的 DataNode 等
    2）DataNode（DN）：在本地文件系统存储文件块数据，以及块数据的校验和
    3）Secondary NameNode（2NN）：每隔一段时间对 NameNode 元数据备份
* YARN：资源调度管理者
    1）ResourceManager：整个集群资源的老大
    2）NodeManager：单个节点服务器资源老大
    3）ApplicationMaster：单个任务运行的老大
    4）Container：容器，相当一台独立的服务器
* MapReduce：分为两个阶段 Map 和 Reduce
    1）Map：映射
    2）Reduce：汇聚
```
#### 6、 大数据技术生态体系
#### 7、 推荐系统案例
### 1.1.2 环境准备
#### 1、 模板虚拟机准备

hadoop 21集

#### 2、 克隆
#### 3、 安装 JDK、Hadoop
### 1.1.3 Hadoop 生产集群搭建
#### 1、本地模式
#### 2、完全分布式集群
### 1.1.4 常见错误的解决方案