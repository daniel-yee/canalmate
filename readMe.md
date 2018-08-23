## 目的
随着业务对数据实时性要求的提高，业务方有实时同步mysql数据的需求，经过调研后，选择canal做数据同步中间件，把数据实时同步到大数据平台。
canal为阿里巴巴的开源项目，负责异构数据源的实时同步。但canal相关的监控和配置系统比较薄弱，相关的运维工作是手动登录到指定机器上以命令行的方式进行。若后期canal方案成熟后，大规模应用到mysql数据库上，canal监控和运维的工作会大幅增加。若没有一个web版的监控和运维系统，会大大降低canal集群的监控和使用效率，这也是团队在使用和运维canal过程中的痛点。
基于以上现状，我们决定做统一的canal运维和监控的系统，满足下面的需求：
- 数据同步的延迟监控和延迟告警
- canalServer和canalClient进程的监控和告警
- mysql同步库(表)的在线管理（添加，删除，过滤同步表和库）

## 系统功能
- 进程管理
- 延迟监控
- 配置管理
- 用户管理

## 技术选型 
- 后端框架：Spring Boot 1.5
- 页面交互：Vue2.x

## 软件需求
- JDK1.8+
- MySQL5.5+
- Tomcat7.0+
- Maven3.0+

## 详情介绍，请查看wiki
