# checkpointsave 合并阶段性工作记录

- 用户要求调整 `Skills/checkpointsave/SKILL.md` 的保存记录规则：仅在较大、总体工作或有意义的工作阶段结束时集中记录，避免每次小改动都生成内容很少的独立文件。
- 构建思路：保留原有章节结构和行为意图，统一修改 frontmatter `description`、`Record Work` 与 `Automatic Trigger at Task End` 中互相关联的表述，消除“任何变更都立即建档”的冲突语义。
- 已完成：使用英文加入阶段性集中记录、合并相关变更和避免低内容文件的要求；同步收紧自动触发条件。
- 验证结果：`quick_validate.py` 返回 `Skill is valid!`；目标 Skill 未发现中文字符；`git diff --check` 未发现空白错误，仅有既有 LF/CRLF 换行提示。
- 后续目标：本次仅修改仓库副本；如需跨工作区生效，应另行同步或安装到全局 Skill 目录。
- 工作结束提示：`Checkpoint recorded.`
