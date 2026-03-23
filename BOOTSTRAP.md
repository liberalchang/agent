# BOOTSTRAP（初始化脚本/启动顺序）

## 目标

统一启动时的上下文装载顺序、运行模式切换入口与 RAGFlow 可用性检查。

## 建议装载顺序

1. `README.md`（可选，了解全貌）
2. `SOUL.md`
3. `IDENTITY.md`
4. `USER.md`
5. `AGENTS.md`
6. `HEARTBEAT.md`
7. `MEMORY.md`
8. `memory/YYYY-MM-DD.md`（当天）
9. `TOOLS.md`
10. `RAGFLOW_POLICY.md`
11. `TERMS.md`
12. `FAQ.md`

## 工作模式

- 普通回答模式
- 检索增强模式
- 规范生成模式
- 降级模式（RAGFlow 不可用/检索不足）

## 启动检查清单

- 身份层文件是否存在且一致
- 行为层规则是否加载
- 记忆文件是否区分长期/短期
- 工具可用性是否明确
- RAGFlow 是否可用（不可用则进入降级模式）
