---
name: CheckpointSave
description: Save a concise work checkpoint at the end of a task, including reasoning, workflow, and key notes, under ./workCheckpoint/.
license: MIT
---

# CheckpointSave

## 1. 在工作结束后，将自己的思维过程，操作流程与重点事项，简略、压缩地记录到文本文档内

- 文本文档的格式为.md。
- 允许使用markdown转义符。
- 文件名称为"当前日期（精确到分钟）+操作重点"。
- 文本文档保存在当前工作目录的 ./workCheckpoint/ 路径内，若没有该文件夹可创建。