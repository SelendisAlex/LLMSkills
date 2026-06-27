---
name: archsave
description: Use when the user asks Codex to organize, document, read, or save a project's work architecture, especially when project information is provided and the user explicitly mentions "Organize the Work Architecture" or the Chinese phrase "整理工作架构". Also use when the user asks to briefly summarize today's work, including the Chinese phrase "简述今天工作", so Codex can summarize today's work results from the current day's work records. At task start, read existing workArchitecture/ records when workspace work memory is unavailable or before the first code task, review, or other important task in a session if those records have not been read. When saving architecture documentation, include the project's overall construction strategy, major objective steps, smaller objective workflows, and relevant follow-up work ideas for future interruption, continuation, or handoff.
license: MIT
---

# ArchSave

## Mandatory Startup Check

Before answering or editing for any coding, review, architecture, debugging, project-rule, or other important workspace task:

Read or modify files using UTF-8 encoding.

1. If this is the first code task, review, or other important task in the current workspace/session, or workspace work memory is unavailable, read this skill first.
2. Read all existing Markdown files under `./workArchitecture/` if the directory exists.
3. Treat those architecture records as active workspace context before continuing.
4. If the directory does not exist, continue without creating it unless a work architecture document must be saved later.

## 1. Architecture Documentation Workflow

- Use this skill to gather project context and save durable architecture documentation for future development work.
- Keep the generated document focused on project structure, framework choices, development workflow, important files, and maintenance notes.
- Record architecture documentation in Chinese.
- Preserve the project's overall construction strategy, organized into major objective steps and subdivided into smaller objective workflows, so work can be interrupted and resumed at any time.
- When saving architecture documentation, automatically include relevant follow-up work ideas when they help future continuation or handoff.
- Save the document in a separate folder under the current working directory unless the user specifies another location.

## 2. When the User Provides Project Information and Explicitly Mentions "Organize the Work Architecture" or the Chinese Phrase "整理工作架构"

- Read the project's documentation and understand the project's framework. In short, comprehensively gather information about the project. Then inspect and organize information such as the site's structure under the local directory. After that, compile a development technical document that makes it easier to develop this site project and includes all important information about the site and the open-source project. Save it in a separate folder under the current working directory.

## 3. When the User Mentions "Summarize Today's Work" or the Chinese Phrase "简述今天工作"

- Use the current day's work records to summarize today's work results as one paragraph.
- If today's work contains large or important changes, make the summary appropriately longer while keeping it focused on outcomes.
