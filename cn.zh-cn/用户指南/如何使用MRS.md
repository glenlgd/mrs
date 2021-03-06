# 如何使用MRS<a name="ZH-CN_TOPIC_0173178534"></a>

MRS是一个在华为云上部署和管理Hadoop系统的服务，一键即可部署Hadoop集群。MRS提供租户完全可控的企业级大数据集群云服务，轻松运行Hadoop、Spark、HBase、Kafka、Storm等大数据组件。

MRS使用简单，通过使用在集群中连接在一起的多台计算机，您可以运行各种任务，处理或者存储（PB级）巨量数据。MRS的基本使用流程如下：

1.  开发数据处理程序，MRS的[开发指南](https://support.huaweicloud.com/devg-mrs/mrs_06_0002.html)为用户提供代码示例和教程，帮助您快速开始开发自己的程序并正常运行。
2.  上传程序和数据文件到对象存储服务（OBS）中，用户需要先将本地的程序和数据文件上传至OBS中。
3.  [创建集群](创建集群.md)，用户可以指定集群类型用于离线数据分析和流处理任务，指定集群中预置的弹性云服务器实例规格、实例数量、数据盘类型（普通IO、高 IO、超高 IO）、要安装的组件（Hadoop、Spark、HBase、Hive、Kafka、Storm等）。用户可以使用[引导操作](引导操作简介.md)在集群启动前（或后）在指定的节点上执行脚本，安装其他第三方软件或修改集群运行环境等自定义操作。
4.  [管理作业](作业简介.md)，MRS为用户提供程序执行平台，程序由用户自身开发，MRS负责程序的提交、执行和监控。
5.  [管理集群](查看集群基本信息.md)，MRS为用户提供企业级的大数据集群的统一管理平台，帮助用户快速掌握服务及主机的健康状态，通过图形化的指标监控及定制及时的获取系统的关键信息，根据实际业务的性能需求修改服务属性的配置，对集群、服务、角色实例等实现一键启停等操作。
6.  [删除集群](删除集群.md)，如果作业执行结束后不需要集群，可以删除MRS集群。集群删除后不再产生费用。

