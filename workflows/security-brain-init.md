---
model: claude-sonnet-4-6
type: workflow
domain: security
source: gbrain (garrytan/gbrain)
---

# 🔒 Workflow: Security Brain Init

> Bootstrap: ingest asset inventory → past incidents → CVE feeds → crons

## Overview

End-to-end **Security & Compliance** workflow based on the
**Threat Intelligence Brain** approach from _gbrain (garrytan/gbrain)_.

## Start

```bash
/workflows:security-brain-init [target] [--scope full|quick] [--output md|json|html]
```

## Dashboard

```
╔══════════════════════════════════════════════════════════╗
║  WORKFLOW: SECURITY-BRAIN-INIT                          ║
╠══════════════════════════════════════════════════════════╣
║  Step 1/5  Discovery        ✓  Completed                 ║
║  Step 2/5  Analysis         ✓  Completed                 ║
║  Step 3/5  Planning         ⟳  Running …                 ║
║  Step 4/5  Execution        ░  Pending                   ║
║  Step 5/5  Report           ░  Pending                   ║
╠══════════════════════════════════════════════════════════╣
║  [████████████░░░░░░░░]  60%   ETA: ~12 min              ║
╚══════════════════════════════════════════════════════════╝
```

## Completion Report

```markdown
## Security Brain Init — Report

**Date:** {date}  **Duration:** {duration}

### Summary
{2-3 sentence executive summary}

### Findings
| Priority | Finding | Owner | Due |
|----------|---------|-------|-----|

### Metrics
| Metric | Before | After | Δ |
|--------|--------|-------|---|
```
