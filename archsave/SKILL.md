---
name: archsave
description: Use when the user asks Codex to organize, document, read, or save a project's work architecture, especially when project information is provided and the user explicitly mentions "Organize the Work Architecture". At task start, read existing workArchitecture/ records when workspace work memory is unavailable or before the first code task, review, or other important task in a session if those records have not been read.
license: MIT
---

# ArchSave

## Mandatory Startup Check

Before answering or editing for any coding, review, architecture, debugging, project-rule, or other important workspace task:

1. If this is the first code task, review, or other important task in the current workspace/session, or workspace work memory is unavailable, read this skill first.
2. Read all existing Markdown files under `./workArchitecture/` if the directory exists.
3. Treat those architecture records as active workspace context before continuing.
4. If the directory does not exist, continue without creating it unless a work architecture document must be saved later.

## 1. Architecture Documentation Workflow

- Use this skill to gather project context and save durable architecture documentation for future development work.
- Keep the generated document focused on project structure, framework choices, development workflow, important files, and maintenance notes.
- Save the document in a separate folder under the current working directory unless the user specifies another location.

## 2. When the User Provides Project Information and Explicitly Mentions "Organize the Work Architecture"

- Read the project's documentation and understand the project's framework. In short, comprehensively gather information about the project. Then inspect and organize information such as the site's structure under the local directory. After that, compile a development technical document that makes it easier to develop this site project and includes all important information about the site and the open-source project. Save it in a separate folder under the current working directory.
