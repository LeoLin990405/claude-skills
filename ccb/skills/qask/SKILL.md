---
name: qask
description: Async via qask, end turn immediately; use only when user explicitly delegates to Qwen (ask/@qwen/let qwen/review); NOT for questions about Qwen itself.
metadata:
  short-description: Ask Qwen asynchronously via qask
  managed-by: ccb-installer
  template-variant: bash
---

# Ask Qwen (Async)

Send the user's request to Qwen asynchronously.

## Execution (MANDATORY)

```
Bash(qask <<'EOF'
$ARGUMENTS
EOF
, run_in_background=true)
```

## Rules

- After running `qask`, say "Qwen processing..." and immediately end your turn.
- Do not wait for results or check status in the same turn.

## Notes

- If it fails, check backend health with `qping`.
