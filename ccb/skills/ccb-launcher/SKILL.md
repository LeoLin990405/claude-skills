---
name: ccb-launcher
description: Launch and manage CCB (Claude Code Bridge) multi-AI collaboration environment. Use when user wants to start CCB, check CCB status, launch WezTerm, configure CCB providers, or troubleshoot CCB environment issues. Handles WezTerm launching, CCB startup, provider configuration, and environment validation.
---

# CCB Launcher

Automated CCB (Claude Code Bridge) environment setup and launch management.

## Overview

This skill handles the complete workflow for starting CCB multi-AI collaboration:
1. Environment validation
2. WezTerm launching
3. CCB startup with configured providers
4. Status monitoring and troubleshooting

## When to Use

Trigger this skill when user:
- Asks to "start CCB" or "launch CCB"
- Wants to "open WezTerm"
- Needs to check CCB status
- Has CCB environment issues
- Wants to configure CCB providers

## Quick Start

### Start CCB (Complete Workflow)

```bash
# 1. Validate environment
ccb -v

# 2. Open WezTerm (if not already in WezTerm)
open -a WezTerm

# 3. In WezTerm terminal, start CCB
ccb

# Or with specific providers
ccb codex gemini
```

## Core Workflows

### Workflow 1: Check CCB Status

```bash
# Check CCB installation and version
ccb -v

# Check configuration
cat ~/.ccb/ccb.config

# Check available commands
which cask gask oask iask kask qask dskask dask
```

### Workflow 2: Launch WezTerm

**macOS:**
```bash
# Method 1: Using open command
open -a WezTerm

# Method 2: Using WezTerm CLI
wezterm start

# Method 3: Check if already in WezTerm
echo $TERM_PROGRAM
# Should output: WezTerm
```

**Detection:**
```bash
# Detect if running in WezTerm
if [ "$TERM_PROGRAM" = "WezTerm" ]; then
    echo "✅ Running in WezTerm"
else
    echo "❌ Not in WezTerm - Opening WezTerm..."
    open -a WezTerm
fi
```

### Workflow 3: Start CCB with Providers

**Using ccb.config (Recommended):**
```bash
# CCB reads from ~/.ccb/ccb.config
ccb

# Example config:
# codex,gemini,opencode,claude,cmd
```

**Manual provider specification:**
```bash
# Two AI providers
ccb codex gemini

# All nine AI providers (including Droid)
ccb codex gemini opencode iflow kimi qwen deepseek droid claude

# With command pane
ccb codex gemini cmd

# With flags
ccb -r              # Resume session
ccb -a              # Auto-approval mode
ccb -a -r codex     # Combined flags
```

### Workflow 4: Validate Environment

**Pre-flight checks:**
```bash
# 1. Check WezTerm installation
which wezterm
wezterm --version

# 2. Check CCB installation
which ccb
ccb -v

# 3. Check Python version
python3 --version
# Should be 3.10+

# 4. Check collaboration commands
which cask gask oask iask kask qask dskask dask cping gping oping iping kping qping dskping dping

# 5. Check configuration
ls -la ~/.ccb/
cat ~/.ccb/ccb.config
```

### Workflow 5: Troubleshoot Issues

**Common issues and solutions:**

**Issue 1: "CCB must run inside tmux or WezTerm"**
```bash
# Solution: Launch WezTerm first
open -a WezTerm
# Then run CCB in WezTerm terminal
```

**Issue 2: Python version too old**
```bash
# Check version
python3 --version

# If < 3.10, upgrade
brew install python@3.13

# Add to PATH in ~/.zshrc or ~/.bashrc
export PATH="/opt/homebrew/opt/python@3.13/libexec/bin:$PATH"

# Reload shell
source ~/.zshrc
```

**Issue 3: CCB commands not found**
```bash
# Check PATH
echo $PATH | tr ':' '\n' | grep .local/bin

# If missing, add to ~/.zshrc or ~/.bashrc
export PATH="$HOME/.local/bin:$PATH"

# Reload
source ~/.zshrc
```

**Issue 4: Configuration not found**
```bash
# Create global config
cat > ~/.ccb/ccb.config << 'EOF'
codex,gemini,opencode,iflow,kimi,qwen,deepseek,claude,cmd
EOF

# Or create project-specific config
mkdir -p .ccb_config
cat > .ccb_config/ccb.config << 'EOF'
codex,gemini,iflow,kimi,qwen,deepseek
EOF
```

## Decision Tree

```
User wants to use CCB?
│
├─ Check: Is CCB installed?
│  ├─ No → Guide installation
│  └─ Yes → Continue
│
├─ Check: Running in WezTerm/tmux?
│  ├─ No → Launch WezTerm
│  │       open -a WezTerm
│  │       (Tell user to run CCB in new WezTerm window)
│  └─ Yes → Continue
│
├─ Check: Environment valid?
│  ├─ Python < 3.10 → Guide upgrade
│  ├─ Missing commands → Check PATH
│  └─ All good → Continue
│
├─ Check: Configuration exists?
│  ├─ No → Create ~/.ccb/ccb.config
│  └─ Yes → Continue
│
└─ Start CCB
   ├─ Use config: ccb
   ├─ Specific providers: ccb codex gemini
   ├─ Resume session: ccb -r
   └─ Auto mode: ccb -a
```

## Execution Steps

When user asks to start CCB, follow these steps:

### Step 1: Validate Environment

```bash
# Run validation checks
ccb -v
python3 --version
echo $TERM_PROGRAM
```

**Parse output to determine:**
- ✅ CCB version
- ✅ Python version
- ✅ Current terminal

### Step 2: Handle Terminal

**If not in WezTerm:**
```bash
# Launch WezTerm
open -a WezTerm

# Tell user:
# "✅ WezTerm launched. Please run 'ccb' in the new WezTerm window."
# END TURN (cannot continue in same shell)
```

**If in WezTerm:**
```bash
# Continue to next step
echo "✅ Running in WezTerm"
```

### Step 3: Check Configuration

```bash
# Check if config exists
if [ -f ~/.ccb/ccb.config ]; then
    cat ~/.ccb/ccb.config
else
    # Create default config
    cat > ~/.ccb/ccb.config << 'EOF'
codex,gemini,opencode,claude,cmd
EOF
    echo "✅ Created default CCB config"
fi
```

### Step 4: Provide Launch Instructions

**IMPORTANT:** Cannot start CCB directly from this shell because:
- CCB requires WezTerm/tmux
- CCB creates split panes
- Must be run interactively by user

**Instead, provide clear instructions:**
```bash
cat << 'EOF'
🚀 Ready to start CCB!

Run this command in WezTerm:
    ccb

Or with specific providers:
    ccb codex gemini

Or resume previous session:
    ccb -r

The terminal will split into multiple panes:
┌─────────┬─────────┬─────────┬─────────┐
│ Codex   │ Gemini  │ OpenCode│ DeepSeek│
├─────────┼─────────┼─────────┼─────────┤
│ iFlow   │  Kimi   │  Qwen   │ Claude  │
├─────────┴─────────┴─────────┴─────────┤
│           CCB-Cmd (bash)              │
└───────────────────────────────────────┘
EOF
```

### Step 5: Post-Launch Verification

After user starts CCB, verify:

```bash
# Check CCB is running
ps aux | grep ccb | grep -v grep

# Test connections
cping    # Test Codex
gping    # Test Gemini
oping    # Test OpenCode
iping    # Test iFlow
kping    # Test Kimi
qping    # Test Qwen
dskping  # Test DeepSeek
dping    # Test Droid
```

## Common Use Cases

### Use Case 1: First-time CCB Launch

**User says:** "Start CCB"

**Actions:**
1. Check environment (`ccb -v`, `python3 --version`)
2. Launch WezTerm (`open -a WezTerm`)
3. Tell user: "✅ WezTerm launched. Run 'ccb' in the new window."

### Use Case 2: Quick Start (Already in WezTerm)

**User says:** "Launch CCB with Codex and Gemini"

**Actions:**
1. Verify in WezTerm (`echo $TERM_PROGRAM`)
2. Provide command: `ccb codex gemini`
3. Explain what will happen (split panes)

### Use Case 3: Troubleshooting

**User says:** "CCB won't start"

**Actions:**
1. Run diagnostics
2. Identify issue (Python, terminal, PATH, config)
3. Provide solution
4. Verify fix

### Use Case 4: Resume Session

**User says:** "Resume my CCB session"

**Actions:**
1. Check if sessions exist (`ls ~/.ccb/sessions`)
2. Provide command: `ccb -r`
3. Explain session restoration

## Reference Commands

### CCB Commands
```bash
ccb              # Start with config
ccb -h           # Help
ccb -v           # Version
ccb -r           # Resume
ccb -a           # Auto-approve
ccb update       # Update CCB
ccb update cca   # Update CCA
```

### Environment Commands
```bash
open -a WezTerm           # Launch WezTerm
wezterm --version         # Check WezTerm
ccb -v                    # Check CCB
python3 --version         # Check Python
which cask gask oask      # Check commands
```

### Configuration
```bash
cat ~/.ccb/ccb.config                # View global config
cat .ccb_config/ccb.config           # View project config
ls ~/.ccb/sessions                   # View sessions
```

## Best Practices

1. **Always validate environment first**
   - Check CCB, Python, WezTerm versions
   - Verify commands are in PATH

2. **Launch WezTerm before CCB**
   - CCB requires terminal multiplexer
   - Cannot start CCB from non-WezTerm shell

3. **Use configuration files**
   - Prefer `~/.ccb/ccb.config` over manual flags
   - Create project-specific configs when needed

4. **Handle errors gracefully**
   - Provide clear error messages
   - Suggest specific solutions
   - Verify fixes work

5. **Explain what's happening**
   - Tell user what command to run
   - Explain expected behavior (split panes)
   - Confirm successful launch

## Error Handling

### Common Errors

**Error:** "CCB must run inside tmux or WezTerm"
```bash
# Solution
open -a WezTerm
# Then tell user to run CCB in WezTerm
```

**Error:** "Missing dependency: python (3.10+ required)"
```bash
# Solution
brew install python@3.13
export PATH="/opt/homebrew/opt/python@3.13/libexec/bin:$PATH"
source ~/.zshrc
```

**Error:** "command not found: ccb"
```bash
# Solution
export PATH="$HOME/.local/bin:$PATH"
source ~/.zshrc
# Or reinstall CCB
```

**Error:** "No configuration found"
```bash
# Solution
cat > ~/.ccb/ccb.config << 'EOF'
codex,gemini,opencode,iflow,kimi,qwen,deepseek,claude,cmd
EOF
```

## Notes

- **Cannot execute CCB directly**: This skill prepares the environment but cannot start CCB itself (requires interactive WezTerm session)
- **WezTerm is required**: CCB needs terminal multiplexing for split panes
- **Configuration is key**: Proper config makes CCB launch seamless
- **Session persistence**: Use `-r` flag to maintain AI context across restarts
