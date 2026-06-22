# firstinit 架构职责迁移到 archsave

- 修改 `Skills/firstinit/SKILL.md`：删除第 4 条“Organize the Work Architecture”相关内容，并从 description 中移除首次项目架构准备职责。
- 新增并整理 `archsave/SKILL.md`：补齐规范 frontmatter、标题、架构文档工作流，并将原 `firstinit` 第 4 条作为 `archsave` 第 2 条。
- 运行 `skill-creator` 的 `quick_validate.py` 校验 `archsave` 与 `Skills/firstinit`，结果均为 `Skill is valid!`。
- 运行 `git diff --check`，仅出现既有 Git 换行规范提示，无 whitespace 错误。
