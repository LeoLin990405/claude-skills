---
name: kask
description: Async via kask, end turn immediately; use only when user explicitly delegates to Kimi (ask/@kimi/let kimi/review); NOT for questions about Kimi itself.
metadata:
  short-description: Ask Kimi asynchronously via kask
  managed-by: ccb-installer
  template-variant: bash
---

# Ask Kimi (Async)

Send the user's request to Kimi asynchronously.

## Execution (MANDATORY)

```
Bash(kask <<'EOF'
$ARGUMENTS
EOF
, run_in_background=true)
```

## Rules

- After running `kask`, say "Kimi processing..." and immediately end your turn.
- Do not wait for results or check status in the same turn.

## Notes

- If it fails, check backend health with `kping`.
