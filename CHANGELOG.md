# 更新日志

本项目的所有重要变更都记录在这里。格式参考 [Keep a Changelog](https://keepachangelog.com/zh-CN/1.1.0/)。

## [1.0.0] - 2026-11-13

### 新增
- 首个 Skill 版发布：把原 ZCode 动态工作流 [`MRqok/ai-gm-team`](https://github.com/MRqok/ai-gm-team) 的「总经理工作模式」重写成平台无关的 Agent Skill。
- `SKILL.md`：frontmatter（name / description / whenToUse）+ 何时用/不用、三角色、七阶段主流程、数据契约、交付报告规范、平台适配与降级说明。
- `references/prompts.md`：三个人设全文、7 个阶段的提问模板、数据结构、成果路径规则、进度板、老板请示机制。
- `references/usage-examples.md`：下达任务的说法、参数调节、典型/不适用场景、质量与诚实性约定。
- `README.md` / `LICENSE`（MIT）/ `.gitignore`。

### 变更（相对旧版）
- **不再绑定 ZCode**：去掉 `.dwf.ts` 工作流引擎、专有 `agent()` / `artifact.board()` / `phase()` API 与独立版 Web 应用。
- **可移植**：派生子 Agent、并行、进度展示、文件落盘全部写成可选适配；无对应能力时给出降级路径。
- **保留**：总经理负责制、员工真实分工、逐包打开验收打回返工、独立审读员冷读、老板请示机制、诚实交付、可调参数（maxWorkers / maxRounds）。

### 说明
- 旧仓库 `MRqok/ai-gm-team` 保持原样，继续提供 ZCode 工作流与独立版 Web 应用；本仓库是其 Skill 版重写，两者并存。
