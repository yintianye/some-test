# Kafka Evolution Task

* 预研Kafka 3.2.0、kafka 2.8.1 两版本与现有kafka 2.0.0的兼容性
  * 部署、使用kafka 3.2.0及2.8.1版本
  * 确定兼容性
    * 是否可使用某一版本的java kafka-clients同时收发3.2.0 and 2.0.0的消息
    * 若上述不可行，改为2.8.1 and 2.0.0兼容
    * 修改kafka-starter 2.0.0-SNAPSHOT版本以支持上述多kafka集群连接
  * 编写相应部署文档和代码文档
* kafka监控
  * 若3.2.0版本可行，须改造kafka-exporter以支持对新版本的监控能力
  * 服务治理中，继续实现consumer—topic—latency告警细粒度配置功能【optional】