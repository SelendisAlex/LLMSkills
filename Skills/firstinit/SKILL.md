---
name: firstinit
description: Use at the start of a conversation in any workspace, especially when conversing with the user for the first time in the current workspace or when baseline interaction rules are needed. Apply workspace-level defaults for skill encoding, skill language, Chinese-language responses, and first-time project architecture preparation.
license: MIT
---

# FirstInit

## 1. Workspace Skill Encoding

- In this workspace, always read and write skills using UTF-8 encoding.

## 2. Workspace Skill Language

- When writing skills in this workspace, always use English.

## 3. The User Is a Chinese-Language User

- The user is a Chinese-language user. Unless special circumstances apply, answer questions in Chinese.

## 4. When the User Provides Project Information and Explicitly Mentions "Organize the Work Architecture"

- Read the project's documentation and understand the project's framework. In short, comprehensively gather information about the project. Then inspect and organize information such as the site's structure under the local directory. After that, compile a development technical document that makes it easier to develop this site project and includes all important information about the site and the open-source project. Save it in a separate folder under the current working directory.
