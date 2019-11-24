# mall
# 采用消息队列解决高并发下单案例, 基于Java语言来开发（JDK1.8） #

## Features ##
1. 采用微服务框架Spring Boot，Spring Cloud，消息队列RabbitMQ搭建解决高并发下单的案例.
2. 集成Spring Cloud的Eureka注册中心，Config分布式配置中心，Ribbon和RestTemplate，Feign负载均衡组件，Hystrix熔断隔离限流降级组件，Zipkin链路跟踪组件等，提高调用服务的简便性.
3. 订单服务采用数据库中间件Sharding-JDBC水平分表，读写分离，解决数据库的吞吐量瓶颈问题，同时采用CQ两端架构上层代码分离[读写分离]，解决复杂的业务逻辑，实现松耦合，可扩展性.
4. 网关服务结合阿里巴巴分布式配置管理Nacos实现动态路由，即不重启网关服务动态的对应路由的配置和规则进行操作.
5. 基于Ntty 4.x实现WebSocket长连接服务，支持在线聊天(群聊，私聊)功能，支持百度云LSS在线直播，支持高并发，高性能.
6. 集成APM-Apache SkyWalking对调用进行分布式追踪、性能指标分析、应用和服务依赖分析，Java自动探针零侵入支持，遵循Tracing的Opentracing规范标准.
7. 集成增强版Swagger-ui可视化界面可以快速体验.

## 架构图 ##
![](F:/architecture.jpg)
`注:架构图中部分技术点还未对接，后续会陆续完成.`

## Prerequisite ##
1. JDK 1.8+
2. Maven 3.5.x
3. Git版本控制

## Quick Start ##
- Clone & Build
> git clone https://github.com/fengjingwei/mall.git
> 
> cd mall
> 
> mvn -DskipTests clean install -U

- execute sql
>  [https://github.com/fengjingwei/mall/blob/master/sql/mall_create_tables.sql](https://github.com/fengjingwei/mall/blob/master/sql/mall_create_tables.sql)

## Support ##
- 如有任何问题欢迎微我
- ![](https://i.imgur.com/8HEEH6x.jpg)
