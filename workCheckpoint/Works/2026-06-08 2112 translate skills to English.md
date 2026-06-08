# Translate Skills to English

- Translated the workspace skill files `Skills/firstinit/SKILL.md` and `Skills/checkpointsave/SKILL.md` from Chinese to English.
- Preserved the original skill structure, front matter, paths, and behavioral intent.
- Verified with `rg -n "\p{Han}"` that no Chinese characters remain in the workspace files.
- Verified with `git diff --check`; only Git line-ending normalization warnings were reported.
