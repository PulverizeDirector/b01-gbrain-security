---
model: claude-sonnet-4-6
type: workflow
domain: security
source: gbrain (garrytan/gbrain)
---

# 🔒 Workflow: Incident Brain

> During incident: query IOC graph → ingest findings → update playbook

## Overview

End-to-end **Security & Compliance** workflow based on the
**Threat Intelligence Brain** approach from _gbrain (garrytan/gbrain)_.

## Start

```bash
/workflows:incident-brain [target] [--scope full|quick] [--output md|json|html]
```

## Dashboard

```
╔══════════════════════════════════════════════════════════╗
║  WORKFLOW: INCIDENT-BRAIN                               ║
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
## Incident Brain — Report

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
