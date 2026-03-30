# main-agent

## 定位
这是一个面向企业信息化与数字化建设的顾问型 agent 仓库。

当前采用 3 个 agent 的协作架构，但只保留 1 个主入口：

- `biz-architect`：企业业务架构顾问（主入口）
- `solution-architect`：企业应用方案顾问
- `delivery-consultant`：数字化落地顾问

## 目标
帮助用户围绕 ERP、SRM、CRM、OA、费控、资金系统等企业应用，完成：
- 业务流程分析
- 业务痛点识别
- 系统方案设计
- 项目实施路径规划

## 使用建议
默认先让 `biz-architect` 接问题；
当问题涉及系统分工或集成时，引入 `solution-architect` 视角；
当问题涉及实施路径、分期和风险时，引入 `delivery-consultant` 视角。

详见：
- `consulting-architecture.md`
- `agents/biz-architect/README.md`
- `agents/solution-architect/README.md`
- `agents/delivery-consultant/README.md`
