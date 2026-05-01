# Hermes Skill Governance

> Skill Governance 集成项目 — skill-factory 模式检测 + skill-governance 审批体系
> 
> 📄 知识库: `/mnt/f/04_Obsidian/ai-agent/projects/skill-governance-integration.md`
> 🔗 GitHub: https://github.com/duanhaoyu88/hermes-skill-governance

## 目标

将 skill-factory 的**模式检测能力**与 skill-governance 的**审批质量体系**整合，实现：
- 自动发现重复工作流 → 向用户建议固化 → 走审批流程 → 按标准创建

## 路线图

### Phase 1: 稳定治理 ✅
- [x] SKILL_GOVERNANCE.md 治理文档
- [x] SOUL.md 审批协议
- [x] config.yaml skills.disabled 禁用机制
- [x] skill-governance 操作手册（6 个操作）

### Phase 2: 质量闭环 🔄
- [x] 修复 9 个 description 损坏
- [ ] 补全所有可用 skill 的 when_to_use + Core Principle
- [ ] 建立 skill 使用频率监控
- [ ] Git 追踪 skills/ 目录变更

### Phase 3: 模式发现 ⏳
- [ ] 设计工具调用序列记录机制
- [ ] 实现重复模式检测算法
- [ ] 集成到 skill-governance 操作 7

### Phase 4: 自动化建议 ⏳
- [ ] 「建议新建 skill」通知
- [ ] 模式摘要自动生成
- [ ] 微信平台集成

## 架构约束

- ❌ 不复活 skill-factory 的自动创建行为
- ✅ 检测归检测，审批归审批
- ✅ 新代码从零设计，不继承 skill-factory
- ✅ 所有变更走 skill-governance 审批链

## 关联

- 治理文档: `~/.hermes/SKILL_GOVERNANCE.md`
- 行为准则: `~/.hermes/SOUL.md`
- 操作手册: `~/.hermes/skills/skill-governance/SKILL.md`
- 知识库: `/mnt/f/04_Obsidian/ai-agent/projects/skill-governance-integration.md`
