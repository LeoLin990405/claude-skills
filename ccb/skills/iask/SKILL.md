---
name: iask
description: Async via iask, end turn immediately; use only when user explicitly delegates to iFlow (ask/@iflow/let iflow/review); NOT for questions about iFlow itself.
metadata:
  short-description: Ask iFlow asynchronously via iask
  managed-by: ccb-installer
  template-variant: bash
---

# Ask iFlow (Async)

Send the user's request to iFlow asynchronously.

## Execution (MANDATORY)

```
Bash(iask <<'EOF'
$ARGUMENTS
EOF
, run_in_background=true)
```

## Rules

- After running `iask`, say "iFlow processing..." and immediately end your turn.
- Do not wait for results or check status in the same turn.

## Notes

- If it fails, check backend health with `iping`.
