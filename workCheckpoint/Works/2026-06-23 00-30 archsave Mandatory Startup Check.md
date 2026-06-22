# archsave Mandatory Startup Check

- 修改 `archsave/SKILL.md`，将此前新增的 `Automatic Trigger at Task Start` 条目改为 `Mandatory Startup Check`。
- 参考 `checkpointsave` 的启动检查结构，补充启动前说明句和编号步骤。
- 启动检查现在要求在重要任务前读取当前 skill，并在 `./workArchitecture/` 存在时读取其中 Markdown 文件，将架构记录作为活动上下文。
- 原“Organize the Work Architecture”条目调整回第 2 条。
- 运行 `quick_validate.py .\archsave`，结果为 `Skill is valid!`。
- 运行 `git diff --check`，仅出现既有 Git 换行提示，无 whitespace 错误。
