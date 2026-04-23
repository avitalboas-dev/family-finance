---
name: Family Finance project overview
description: Key facts about the family-finance app — stack, deployment, storage, and open work
type: project
originSessionId: 93f74eab-0e85-4868-9ad0-206053d29e9d
---
Single-file app (index.html + revolut-categories.json) for tracking Revolut CSV exports.

**Repo:** https://github.com/avitalboas-dev/family-finance  
**Live:** https://avitalboas-dev.github.io/family-finance/ (GitHub Pages, main branch)

**Storage:**
- Transactions: localStorage per device (replaced on new CSV upload)
- Categories: JSONBin.io bin `69e9fb5b36566621a8e2bab1` — auto-loads on startup, auto-saves on every category change. Shared across all devices including wife's.

**Why:** Two users (owner + wife), each uploads their own CSV, but category mappings should be shared and zero-setup.

**How to apply:** Push directly to main — no PR/branch workflow. gh CLI is installed and authenticated.
