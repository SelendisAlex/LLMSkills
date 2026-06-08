---
name: checkpointsave
description: Save a concise work checkpoint at the end of a task, including reasoning, workflow, and key notes, under ./workCheckpoint/.
license: MIT
---

# CheckpointSave

## 1. 在每次重要地、长期地或特殊地改动、更新工作结束后，将操作流程与重点事项，简略、压缩地记录到文本文档内，就像检查点一样，并且在回答中汇报：“已记录检查点”

- 文本文档的格式为.md。
- 允许使用markdown转义符。
- 文件名称为"当前日期（精确到分钟）+操作重点"。
- 文本文档保存在当前工作目录的 ./workCheckpoint/ 路径内，若没有该文件夹可创建。

## 2. 自动触发

当任务结束时，如果满足以下任一条件，应自动使用本技能：

- 创建了新的源码文件或模块。
- 修改了 3 个或更多项目文件。
- 新增了功能、子系统、命令、数据库/存储结构，或持久化数据格式。
- 修改了编译、构建、运行时接入逻辑，例如 include、callback、路由、迁移或配置。
- 用户明确强调了未来维护、交接、编码、项目规范，或“记录/记住/checkpoint”。
- 任务中包含不明显的推理过程、发现的重要约束，或需要保留的注意事项。

以下情况不要自动使用：

- 纯问答，没有文件改动。
- 很小的单文件修复。
- 仅格式化改动。
- 临时实验，且最终已回退。

自动触发时，应在最终回复前保存 checkpoint，并在最终回复中简要说明 checkpoint 路径。

- 对于代码任务，在最终回复前检查本次修改的文件数量，以及是否新增模块或持久化格式。
- 如果属于重要改动，应无需询问，直接创建 checkpoint。