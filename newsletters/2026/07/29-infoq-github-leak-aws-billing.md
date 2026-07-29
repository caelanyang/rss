# GitHub Leak, AWS Billing, PixelSmash, Bijou64, React Rust, Jotai v2.20, Mobile AI, Claude

**来源：** InfoQ
**日期：** 2026-07-28
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject:%22GitHub+Leak%2C+AWS+Billing%2C+PixelSmash%2C+Bijou64%2C+React+Rust%2C+Jotai+v2.20%2C+Mobile+AI%2C+Claude%22>

---

## AI/ML 与数据工程

- **Yelp 统一 ML 模型训练：** 使用 Training Orchestrator 统一管理
- **多智能体 AI 安全运营：** 在 5G 核心网中采用 A2A 和 MCP 架构，检测和响应时间减少 40%，人工工作量压缩 12 倍
- **自主数据产品：** 以容器化方式管理数据管道、schema 和元数据，通过 MCP 协议实现渐进式工具发现

## DevOps

- **AWS 计费漏洞：** 配置变更导致部分用户看到数十亿至万亿级别的预估账单持续超过 24 小时。AWS 自身的告警检测到异常但未能阻止账单生成或通知工程师，客户投诉后 4.5 小时才响应
- **AI 根因分析从模型推理转向上下文工程**
- **GitHub AI 智能体遭间接提示注入攻击，泄露私有仓库数据**
- **GitLab 19.2：** AI 智能体用于处理安全积压任务

## 开发

- **Ink & Switch 发布 Bijou64：** 一种规范变长整数编码，每个数字只有唯一种字节表示，关闭了 PKCS#1、JWT 库和比特币中利用规范性问题攻击的漏洞类别。解码速度比 LEB128 快 2-10 倍

## Web 开发

- **Jotai v2.20：** 重构 Store 基础模块以提升高吞吐性能，为 v3 版本做准备
