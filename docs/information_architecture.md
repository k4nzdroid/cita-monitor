# CITA-Monitor 监控指标信息结构

## 链的信息

* 基本信息（不可变的）
    * 创世块生成时间
    * 主网运行时间：最新区块的时间戳 - 创世块生成时间
* 配置信息（可变的）
    * 链名称
    * 链协议版本
    * 经济模型
    * 运营者信息
    * Token符号
* 数据信息（随时间变化的）
    * 最新区块高度
    * 最新区块HASH
    * 最新区块产出距离当前时间（客户端时间戳）
    * 最新区块中经济激励节点主机名或名称（hostname）
    * 最新区块中打包的交易笔数
    * Quota相关信息
        * block limit
        * account quota limit
        * [ ] total quota of a block
        * [ ] total quota used  of a block
        * [ ] sender & receivers
            * [ ] top 5 senders (stack bar)
            * [ ] top 5 receivers (stack bar)
* 节点网络信息
    * 共识节点总数（区分工作中节点、非工作中节点）
    * [ ] 节点分布地图
* 性能相关
    * 出块间隔时间历史记录
    * 平均block产出时间（出块间隔时间历史记录的平均值）
    * 主网每秒请求处理数 TPS（block内交易笔数/平均block产出时间）
    * 柱状图展示区块交易笔数

## 节点信息

* 基本信息（不会变的）
    * 节点id
    * 节点类型：只读，共识
* 节点运行软件信息
    * 节点运行软件版本号
* 运行环境信息
    * 节点运行系统主机名
    * 节点操作系统版本号：如 Ubuntu 16.04
    * 节点IP地址
    * 节点端口号
* 出块信息
    * 节点块高度
    * [ ] 节点未打包的交易笔数
    * 最后出块时间
* 可靠性信息
    * [ ] 节点首次启动时间：时间戳 - cita-forever的日志创建时间
    * [ ] 节点最后启动时间：时间戳 - 从日志分析获取
    * [ ] Peers: 连接的节点总数（区分工作中节点、非工作中节点）
    * [ ] uptime（节点运行时间）：需要每分钟打点
    * 节点存在时间：当前时间 - 节点首次启动时间
    * [ ] 节点运行可靠性：节点运行时间/节点存在时间



## 节点所在主机信息

* CPU 利用率（CITA 的微服务进程）
* 物理内存（CITA 的微服务进程）
* [ ] 网络IO（CITA 的微服务进程）
* 磁盘利用率及容量


