# sentinel-metrics-prometheus

Sentinel Metrics For Prometheus

### 组件简介

> Sentinel + Actuator 的 Spring Boot Starter 实现；主要代码来自 ：
> https://gitee.com/596392912/mica/tree/master/mica-metrics

### 使用说明

##### 1、Spring Boot 项目添加 Maven 依赖

``` xml
<dependency>
	<groupId>com.github.hiwepy</groupId>
	<artifactId>sentinel-metrics-prometheus</artifactId>
	<version>${project.version}</version>
</dependency>
```

##### 2、使用示例

访问本地配置：

http://localhost:8080/actuator/prometheus

```
sentinel_pass_requests_total{application="druid-app", resource ="xxx"} 0.0
sentinel_block_requests_total{application="druid-app", resource ="xxx"} 0.0
sentinel_success_requests_total{application="druid-app", resource ="xxx"} 0.0
sentinel_exception_requests_total{application="druid-app", resource ="xxx"} 0.0
sentinel_requests_latency_seconds{application="druid-app", resource ="xxx"} -0.001
sentinel_current_threads{application="druid-app", resource ="xxx"} -0.001
```

## Jeebiz 技术社区

Jeebiz 技术社区 **微信公共号**、**小程序**，欢迎关注反馈意见和一起交流，关注公众号回复「Jeebiz」拉你入群。

|公共号|小程序|
|---|---|
| ![](https://raw.githubusercontent.com/hiwepy/static/main/images/qrcode_for_gh_1d965ea2dfd1_344.jpg)| ![](https://raw.githubusercontent.com/hiwepy/static/main/images/gh_09d7d00da63e_344.jpg)|
