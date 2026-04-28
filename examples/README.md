# 🔒 Examples — Threat Intelligence Brain

## Quick Command Example

```bash
/threat-ingest my-target --output md
```

**Output:**


```
╔══════════════════════════════════════════════════╗
║  Threat Brain  —  "sql injection campaign"       ║
╠══════════════════════════════════════════════════╣
║  CVE graph …         [██████] 100%   34 CVEs     ║
║  Incident history … [████░░]  80%    12 incidents║
║  ATT&CK mapping …   [██████] 100%                ║
╚══════════════════════════════════════════════════╝

Related threat activity:
  T1190  Exploit Public-Facing App  — 3 past incidents  🔴
  T1505  Server-Side Backdoor       — linked to CVE-2024-1234
  Recommended: WAF rule update + patch nginx 1.24→1.26
```

## Workflow Example

```bash
/workflows:security-brain-init my-target --scope full
```

```
╔══════════════════════════════════════════════════════════╗
║  Step 1/5  Discovery   ✓  Done                          ║
║  Step 2/5  Analysis    ✓  Done                          ║
║  Step 3/5  Planning    ⟳  Running …                    ║
║  [████████████░░░░░░]  60%   ETA ~12 min                ║
╚══════════════════════════════════════════════════════════╝
```

## Tips

1. Start with `/threat-ingest` for a quick overview.
2. Use `--scope quick` for fast scans, `--scope full` for production.
3. Chain: run analysis first → use findings as input for planning.
4. `--output html` generates a stakeholder-ready report.
