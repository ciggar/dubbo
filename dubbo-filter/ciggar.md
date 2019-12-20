dubbo-filter-cache: 缓存热点数据，结果缓存
    用户加速热门数据的访问速度，Dubbo提供声明式缓存，以减少用户加缓存的工作量

配置如下示例：

```xml
<dubbo:reference interface="com.foo.BarService" cache="lru" />
```
或：
```xml
<dubbo:reference interface="com.foo.BarService">
    <dubbo:method name="findBar" cache="lru" />
</dubbo:reference>
```
cache缓存类型可配置：
    lru：基于最近最少使用原则删除多余缓存，保持最热的数据被缓存
    threadlocal：当前线程缓存
    jcache：与JSR107集成，可以桥接各种缓存的实现
    
    
    
dubbo-filter-validation：参数验证模块