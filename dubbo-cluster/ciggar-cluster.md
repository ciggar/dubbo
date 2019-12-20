dubbo-cluster:集群模块
    讲多个服务提供方伪装为一个提供方，包括：负载均衡，集群容错，路由，分组聚合等。
    集群的地址列表可以是静态配置的，也可以是由注册中心下发
    
dubbo-cluster 集群容错
    [http://dubbo.apache.org/zh-cn/docs/user/demos/fault-tolerent-strategy.html] 

dubbo集群容错是指的是在集群调用失败时，dubbo提供了多种容错方案，缺省为 failover 重试。