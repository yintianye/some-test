# Spring Cloud Evolution Task

* 项目地址
  * [archetype](http://gitlab.htffund.com/platform/archetype) 2.0.0-SNAPSHOT 分支
  * [framework-dependency-parent](http://gitlab.htffund.com/platform/COMMON-LIBS/htf-framework-dependency-parent) master分支
* 基线
  * [Spring Cloud](https://spring.io/projects/spring-cloud)  2021.0.3
  * [Spring Boot](https://spring.io/projects/spring-boot)  2.7.0（alternative 2.6.8）
* 涉及改造项【当前已知项，待持续补充】
  * [framework-dependency-parent](http://gitlab.htffund.com/platform/COMMON-LIBS/htf-framework-dependency-parent) 
    * 涉及并完善包管理、插件等相关项
  * eureka
    * 验证并支持多版本spring cloud节点兼容
  * actuator-spring-cloud-starter
    * 多项基础功能改造
    * 【notice】2021.0.3版本FeignClient不允许使用@RequestMapping
  * bee-spring-cloud-starter
    * 支持响应式
  * canary-spring-cloud-starter
    * 细粒度支持灰度
  * gateway-spring-cloud-starter
    * 支持响应式
  * circuit-breaker
    * Resilence4j引入
    * 确认并优化基于Spring Retry的重试机制
  * kafka-spring-cloud-starter
    * 见[Kafka Evolution Task](./kafka.md)
  * monitor-spring-cloud-starter
    * 多项基础监控改造
  * redis-spring-cloud-starter
    * 见[Redis Evolution Task](./redis.md)