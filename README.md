<h1 align="center">Miles Zeng</h1>

<p align="center">
  <b>Java 后端开发</b> · 分布式系统 · AI Agent 工程
</p>

<p align="center">
  计算机专业学生，关注高可靠后端系统、分布式一致性、数据库内核与 AI 原生软件工程。
</p>

<p align="center">
  <a href="https://github.com/zeng1230">
    <img
      alt="GitHub"
      src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white"
    />
  </a>

  <a href="https://github.com/zeng1230/systems-course-showcase">
    <img
      alt="系统课程实践"
      src="https://img.shields.io/badge/系统课程-实践展示-4C1?style=flat&logo=readthedocs&logoColor=white"
    />
  </a>
</p>

---

## 关于我

我目前主要学习和实践 Java 后端开发，同时持续深入数据库、操作系统、计算机网络和分布式系统。

在应用层，我使用 Spring Boot、MySQL、Redis、RabbitMQ 等技术构建后端项目，重点关注事务一致性、缓存并发、消息可靠性、故障恢复和可测试性。

在系统层，我通过 CMU、MIT、Stanford 和 UC Berkeley 的课程实验，实践过数据库内核、TCP 协议栈、RISC-V 操作系统、Raft 共识协议和数据结构。

我也在探索 AI Agent 后端开发，关注模型权限边界、工具调用控制、安全检查、工作流补偿和离线评测。

---

## 技术栈

<p align="center">
  <img
    src="https://skillicons.dev/icons?i=java,spring,mysql,redis,rabbitmq,docker,linux,git,githubactions,maven"
  />
</p>

<p align="center">
  <img
    src="https://skillicons.dev/icons?i=go,cpp,c,python"
  />
</p>

<p align="center">
  <img
    alt="Spring Boot"
    src="https://img.shields.io/badge/Spring%20Boot-6DB33F?logo=springboot&logoColor=white"
  />
  <img
    alt="MyBatis Plus"
    src="https://img.shields.io/badge/MyBatis--Plus-DC382D?logo=java&logoColor=white"
  />
  <img
    alt="Redis"
    src="https://img.shields.io/badge/Redis-DC382D?logo=redis&logoColor=white"
  />
  <img
    alt="RabbitMQ"
    src="https://img.shields.io/badge/RabbitMQ-FF6600?logo=rabbitmq&logoColor=white"
  />
  <img
    alt="Testcontainers"
    src="https://img.shields.io/badge/Testcontainers-2496ED?logo=docker&logoColor=white"
  />
  <img
    alt="Flyway"
    src="https://img.shields.io/badge/Flyway-CC0200?logo=flyway&logoColor=white"
  />
  <img
    alt="JUnit 5"
    src="https://img.shields.io/badge/JUnit%205-25A162?logo=junit5&logoColor=white"
  />
</p>

---

## 代表项目

### Price Tracker 商品价格监控与通知系统

<p>
  <a href="https://github.com/zeng1230/prace_tracker">
    <b>查看项目仓库</b>
  </a>
</p>

<p>
  <img
    src="https://skillicons.dev/icons?i=java,spring,mysql,redis,rabbitmq,docker"
  />
</p>

面向电商商品目标价订阅场景的后端系统，实现商品价格刷新、降价事件生成和订阅通知异步投递。

主要实践：

- 使用 Transactional Outbox 处理业务事务与消息投递的一致性
- 使用 Redis 与 MySQL 唯一约束实现多层幂等控制
- 使用 Lua 分布式锁、Double Check、空值缓存和随机过期时间保护缓存
- 在 HTTP、异步任务和消息消费链路中传递 TraceId
- 使用 Testcontainers 构造真实中间件集成测试环境
- 使用 Flyway 管理数据库结构演进

---

### TravelCare Agent 受控式 AI 旅行客服后端

<p>
  <a href="https://github.com/zeng1230/TravelCare_Agent">
    <b>查看项目仓库</b>
  </a>
</p>

<p>
  <img
    src="https://skillicons.dev/icons?i=java,spring,mysql,redis,rabbitmq"
  />
</p>

面向旅游退款场景构建的受控 AI 客服后端。LLM 负责意图理解和回复润色，后端工作流负责订单查询、规则判断、工具授权、状态变更和异常补偿。

主要实践：

- 将退款流程建模为确定性工作流和状态机
- 限制模型直接执行退款等敏感业务操作
- 实现 ModelSafetyGate 检测违规承诺、隐私泄漏和越权调用
- 使用 Redis 锁和数据库幂等键控制工具重复执行
- 使用对账服务处理 UNKNOWN 状态和外部交易异常
- 实现对象级访问控制、租户数据隔离和敏感信息脱敏
- 设计 Diagnostic Dry Run、Trace Diff 和离线评测流程

---

### Systems Course Showcase 系统课程实践展示

<p>
  <a href="https://github.com/zeng1230/system-course-showcase">
    <b>查看系统课程实践</b>
  </a>
</p>

<p>
  <img
    src="https://skillicons.dev/icons?i=go,cpp,c,java,linux"
  />
</p>

系统课程与工程实践覆盖：

- MIT 6.5840 分布式系统
- CMU 15-445 数据库系统
- MIT 6.S081 操作系统
- Stanford CS144 计算机网络
- Stanford CS146S AI 原生软件工程
- UC Berkeley CS61B 数据结构

实践内容包括：

- Raft 领导者选举、日志复制、持久化与快照
- 分布式 KV 服务与分片迁移
- Buffer Pool、B+ Tree 和查询执行器
- RISC-V xv6 虚拟内存、Copy-on-Write 和锁优化
- TCP Sender、TCP Receiver、ARP 和 IPv4 路由
- 树、哈希表、优先队列与图算法
- AI 辅助开发、测试生成、代码审查和工程工作流

课程源码根据学术诚信要求保存在私有仓库，公开仓库仅展示实验范围、架构理解、测试结果和学习总结。

---
