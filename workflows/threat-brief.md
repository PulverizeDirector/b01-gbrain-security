---
model: claude-sonnet-4-6
type: workflow
domain: security
source: gbrain (garrytan/gbrain)
---

# 🔒 Workflow: Threat Brief

> Weekly threat briefing: new CVEs + active threats + compliance status

## Overview

End-to-end **Security & Compliance** workflow based on the
**Threat Intelligence Brain** approach from _gbrain (garrytan/gbrain)_.

## Start

```bash
/workflows:threat-brief [target] [--scope full|quick] [--output md|json|html]
```

## Dashboard

```
╔══════════════════════════════════════════════════════════╗
║  WORKFLOW: THREAT-BRIEF                                 ║
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
## Threat Brief — Report

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
