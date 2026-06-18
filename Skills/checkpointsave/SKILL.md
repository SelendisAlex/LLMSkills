---
name: checkpointsave
description: Save a concise work checkpoint at the end of a task, including reasoning, workflow, and key notes, under ./workCheckpoint/.
license: MIT
---

# CheckpointSave

## 1. Record Work

- Saving rules: Whenever the user gives important input about this project, such as coding standards, project architecture, file architecture, file or folder naming conventions, variable naming conventions, workflows, or other rules that will have a long-term impact on the project, record them in the directory specified below. Keep the record brief while preserving its core meaning.
- Saving work records: After each change or update is completed, record the operation process and key points in a text document in a brief and compressed form, like a checkpoint. Also report in the response: "Checkpoint recorded."
- Saving rules: Use Chinese to record work rules.
- Saving work records: Use Chinese to record work records.

File saving rules:

- The document format is `.md`.
- Markdown escape characters are allowed.
- The file name must be "current date (accurate to the minute) + operation focus".

- Saving rules: Save documents under the `./workCheckpoint/Rules/` path in the current working directory. If this folder does not exist, it may be created. If previously created records exist in the root directory, move them into this folder.
- Saving work records: Save documents under the `./workCheckpoint/Works/` path in the current working directory. If this folder does not exist, it may be created. If previously created records exist in the root directory, move them into this folder.

## 2. Automatic Trigger at Task Start

If you do not have any memory about work in this workspace, or if this conversation is the first code task, review, or other important task in the session and you have not read the work rules (`workCheckpoint\Rules`) or work records (`workCheckpoint\Works`), read them and remember them. This is important.

## 3. Automatic Trigger at Task End

At the end of a task, automatically use this skill if any of the following conditions are met:

- New source code files or modules were created.
- Three or more project files were modified.
- A feature, subsystem, command, database or storage structure, or persistent data format was added.
- Compilation, build, or runtime integration logic was modified, such as includes, callbacks, routes, migrations, or configuration.
- The user explicitly emphasized future maintenance, handoff, coding, project conventions, or "record/remember/checkpoint".
- The task included non-obvious reasoning, important constraints that were discovered, or notes that need to be preserved.

Do not use this skill automatically in the following cases:

- Pure question answering with no file changes.
- A very small single-file fix.
- Formatting-only changes.
- A temporary experiment that was ultimately reverted.

When triggered automatically, save the checkpoint before the final response and briefly state the checkpoint path in the final response.

- For coding tasks, before the final response, check how many files were modified in this task and whether any modules or persistent formats were added.
- If there is a change, create the checkpoint directly without asking.
