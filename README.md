# 联系方式

- 手机：15601821846
- Email：bowen799923347@gmail.com 
- QQ：799923347

---

# 个人信息

 - 赵宝文/男/1991 
 - 硕士/江南大学计算机科学与技术、本科/盐城工学院计算机科学与技术
 - 工作年限：2.5年
 - 期望职位：Java岗
 - 期望城市：上海、杭州

---

# 工作经历

## 上海挖财 （ 2017年6月 ~ 2019年12月 ）
> 初进入挖财时负责对B端商户的资产进件模块的维护；约半年后开始进入资金存管项目，由于政策及业务原因共对接了恒丰银行两个版本的存管系统，18年1月中旬第一个版本上线，至9月份完全切换历经九个月左右的时间；18年7月份公司组织架构拆分开始着手老进件项目的拆分迁移及重构，项目上线后开始外部资产接入，至18年底，本人主要负责对接我来贷资产；19年初开始享换机租机的合作项目；二季度开始资金路由项目，接入机构资金，本人负责与光大信托的对接；再接着时业务线自营的IRR36业务及小贷资金项目等

### 小贷项目 todo 替换为资金路由项目
对接资金路由平台，将借款资产接入小贷资金，管理接入小贷的资产，包括授信、放款、还款计划、还款及代扣等，业务为资产生命周期中贷中、贷后阶段；  
负责功能更：

- 负责接入层(涉及绑卡、授信、放款、还款、文件)的设计，状态机，无锁编程
- 还款功能开发，包括还款计划查询、发起还款请求等
- 文件同步功能的开发，借款合同、日对账文件等文件同步，文件同步任务设计思想基于事件驱动编程，内部实现基于jdk自带的标准函数式接口

### 极光贷项目
APP端独立借款流程，流程包括四要素绑卡、活体验证、借款人基本信息收集、身份证件上传及授信等，业务为资产生命周期中的贷前阶段，Spring Boot应用，kotlin语言开发。  
负责功能：

- 发起提现功能的开发，使用分布式锁控制并发及重复提现申请提交
- 引入Arrow组件，提供丰富的基于kotlin语言的类型化函数式编程体验
- 因为是直接面向C端的产品，引入sentinel，提供单机的流量控制和熔断降级功能，抵御突发的瞬时流量的冲击，提高系统可用性

### 资产接入模块重构 
重构老的资产接入模块的应用，将老的spring应用升级为springboot应用，在兼容老功能的基础上，解决老项目存在的接口过多、接入流程复杂繁琐的问题，提供一站式接入解决方案。  
负责功能：

- 通过dubbo接口将服务暴露至公司网关，外部团队通过网关接入
- dubbo接口定制Joda-Time序列化协议
- 优化既有外部接入流程，存管、进件一站式接入，降低外部接入成本
- 升级消息队列client，由老版本的kafka升级为公司带事务的消息队列中间件，并适配事务特性编程
- 解决老应用架构外部通知数据丢失及幂等问题

### 资金存管项目 
Spring Boot应用，借款人端资金存管功能，前期接入恒丰移动系统、后期替换为恒丰懒猫系统，借款人借款前开通银行存管账户，绑定四要素，借款申请通过后，资金打入存管账户，借款人将资金由银行存管账户提现至银行卡中。  
负责功能：

- 外部合作团队对接，数据传输加解密、验签
- 借款人h5端无状态登录，借款信息回显，h5页面协议列表展示，四要素检查、风控检查
- 前端流程路由
- 存管渠道恒丰移动、恒丰懒猫一键切换
- 经销商、商户账户提现
- 外部依赖接口监控，使用AOP增强外部接口调用，接口调用数据上报，上报数据通过kafka发送，InfluxDB存储上报数据，根据上报的调用数据对接口异常调用发送报警给相关人员

其他：进件、资金路由、享换机租机担保业务、安心保险征信业务、控台开发......
## 实习 （ 2015年7月 ~ 2015年8月 ）
通过分布式hadoop集群处理网站产生的大量日志。通过分布式存储，按小时保存并以小时为周期定时将上一小时的数据同步到日志分析机上。统计数据按小时更新，统计项包括关键词搜索量PV，网站的浏览量PV，类别访问量，访客数UV（包括新访客数、新访客比例），跳出率等信息供网站管理者分析网站使用。  
责任描述：

- 使用flume进行日志文件的收集数据,传输到HDFS中
- 使用MapReduce对数据进行清洗,再存储
- 使用Hive对清洗后的数据进行多维分析
- 使用sqoop把分析结果导入到mysql中
- 返回链接给Web前端，将结果以图表，表格等多种形式表示出来

---

## 演讲和讲义

 - [Java函数式接口](https://pan.baidu.com/s/1dh0CY5tUslbp7L8t7hEFgA)
 - [单元测试-你不知道的事](https://pan.baidu.com/s/1EkUq784XFYuEsT455LPYOA)

---
# 自我评价
有时过于负能量，看问题的角度可能会过于悲观
# 技能清单

以下均为我熟练使用的技能

- 开发：Java、Kotlin
- 框架：Spring全家桶/Kafka/Mybatis/Arrow
-  消息中间件：Kafka
- RPC：Dubbo
-  熔断降级：Sentinel
- 前端框架：Layui
- 数据库相关：MySQL/Redis
- 版本管理、项目管理：Git/Maven/Gradle
- 单元测试：Junit、Mockito
- 其他：VIM、Linux常用运维
