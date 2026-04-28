        # 🔒 Threat Intelligence Brain

        ![Domain](https://img.shields.io/badge/Domain-Security%20&%20Compliance-red?style=for-the-badge)
        ![Skills](https://img.shields.io/badge/Skills-8-blue?style=for-the-badge)
        ![Workflows](https://img.shields.io/badge/Workflows-3-orange?style=for-the-badge)
        ![Source](https://img.shields.io/badge/Source-gbrain%20(garrytan/gbrain)-grey?style=for-the-badge)
        ![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

        > **Self-wiring knowledge graph for threats, vulnerabilities and security incidents**

        Adapted from **gbrain (garrytan/gbrain)** — _self-wiring AI knowledge graph brain — 29 skills, hybrid search, entity enrichment_

        ---

        ## What This Does

        Security audits, vulnerability management, GDPR/SOC2.

        This collection brings the **Threat Intelligence Brain** approach to Security & Compliance work,
        providing **8 domain-specific skills** and **3 end-to-end workflows**
        with structured output and live progress tracking.

        ---

        ## Skills

        | Skill | Description |
        |-------|-------------|
        | `/threat-ingest` | Ingest threat intel feeds — extract CVEs, threat actors, TTPs and link entities |
| `/vuln-graph` | Build vulnerability relationship graph: CVEs, affected systems, patch status |
| `/incident-security` | Store security incidents with IOCs, timeline, MITRE ATT&CK mapping and backlinks |
| `/compliance-brain` | Track compliance controls, evidence links and gap analysis across frameworks |
| `/asset-ingest` | Ingest asset inventory with risk scores, owner links and exposure backlinks |
| `/pentest-ingest` | Store pentest findings with CVSS scores, remediation links and retest backlinks |
| `/threat-query` | Query brain for threat landscape, attack patterns and defensive recommendations |
| `/cve-monitor` | Detect new CVEs affecting your asset graph and surface to security team |

        ---

        ## Workflows

        | Workflow | Description |
        |----------|-------------|
        | `security-brain-init` | Bootstrap: ingest asset inventory → past incidents → CVE feeds → crons |
| `threat-brief` | Weekly threat briefing: new CVEs + active threats + compliance status |
| `incident-brain` | During incident: query IOC graph → ingest findings → update playbook |

        ---

        ## UI Preview


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

        ---

        ## How It Works

        Every skill follows the same 5-step interaction:

        ```
        ① Scope Confirmation   verify target + options
        ② Live Progress        [████████░░] 80%
        ③ Structured Findings  table sorted by impact (🔴🟠🟡🟢)
        ④ Action Plan          quick wins → medium-term → strategic
        ⑤ Next Steps           suggested follow-up skills
        ```

        ---

        ## Install

        ```bash
        # Copy to Claude skills directory
        cp -r . ~/.claude/skills/b01-gbrain--security/

        # Load in Claude Code session
        /read ~/.claude/skills/b01-gbrain--security/SKILL.md
        ```

        ## Source

        Derived from **gbrain (garrytan/gbrain)** — self-wiring AI knowledge graph brain — 29 skills, hybrid search, entity enrichment.
        Original patterns adapted and domain-specialised for Security & Compliance.

        ---
        MIT License
