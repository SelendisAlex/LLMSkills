# checkpointsave 启动触发审查

- 检查 `Skills/checkpointsave/SKILL.md` 中新增的 `Mandatory Startup Check` 条目和 description。
- 判断方向合理：Skill 的触发主要依赖 frontmatter `description`，因此“任务开始读取工作区记录”的触发条件必须写入 description，而不能只写在正文。
- 修正 description 末尾错误拼接的 `preserved.workCheckpoint/.`，并补充 `in any workspace`，使其更明确表达任何工作区的重要任务开始和结束都应触发。
- 注意：仓库副本变更不会自动同步到已安装的全局技能副本，实际跨工作区生效还需要安装/同步到 Codex 会自动发现的技能目录。
