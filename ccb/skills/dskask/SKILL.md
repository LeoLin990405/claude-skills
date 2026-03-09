---
name: dskask
description: Async via dskask, end turn immediately; use only when user explicitly delegates to DeepSeek (ask/@deepseek/let deepseek/review); NOT for questions about DeepSeek itself.
metadata:
  short-description: Ask DeepSeek asynchronously via dskask
  managed-by: ccb-installer
  template-variant: bash
---

# Ask DeepSeek (Async)

Send the user's request to DeepSeek asynchronously.

## Execution (MANDATORY)

```
Bash(dskask <<'EOF'
$ARGUMENTS
EOF
, run_in_background=true)
```

## Rules

- After running `dskask`, say "DeepSeek processing..." and immediately end your turn.
- Do not wait for results or check status in the same turn.

## Notes

- If it fails, check backend health with `dskping`.
