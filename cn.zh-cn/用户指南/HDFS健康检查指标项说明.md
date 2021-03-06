# HDFS健康检查指标项说明<a name="ZH-CN_TOPIC_0173397605"></a>

## 发送包的平均时间统计<a name="section31306212111516"></a>

**指标项名称**：发送包的平均时间统计

**指标项含义**：HDFS文件系统中DataNode每次执行SendPacket的平均时间统计，如果大于2000000纳秒，则认为不健康。

**恢复指导：**  如果该指标项异常，则需要检查集群的网络速度是否正常、内存或CPU使用率是否过高。同时检查集群中HDFS负载是否过高。

## 服务健康状态<a name="section26290515111534"></a>

**指标项名称：**服务状态

**指标项含义**：检查HDFS服务状态是否正常。如果节点有故障，则认为不健康。

**恢复指导：**如果该指标项异常，建议检查KrbServer、LdapServer、ZooKeeper三个服务的状态是否为异常并处理。然后再检查是否是HDFS SafeMode ON导致的写文件失败，并使用客户端，确认是否无法在HDFS中写入数据，排查HDFS写数据失败的原因。最后参见告警进行处理。

## 检查告警<a name="section38495155111537"></a>

**指标项名称：**  告警信息

**指标项含义**：检查HDFS服务是否存在未清除的告警。如果存在，则认为不健康。

**恢复指导：**如果该指标项异常，请参见告警进行修复。

