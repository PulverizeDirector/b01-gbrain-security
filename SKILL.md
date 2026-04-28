        ---
        name: "b01-gbrain--security"
        description: >
          🔒 Threat Intelligence Brain — Self-wiring knowledge graph for threats, vulnerabilities and security incidents.
          Derived from gbrain (garrytan/gbrain). Security audits, vulnerability management, GDPR/SOC2.
        version: "1.0.0"
        domain: security
        tags: ["security", "compliance", "gdpr", "soc2", "owasp"]
        source_concept: "Threat Intelligence Brain"
        license: MIT
        ---

        # 🔒 Threat Intelligence Brain

        > **Self-wiring knowledge graph for threats, vulnerabilities and security incidents**
        > Derived from _gbrain (garrytan/gbrain)_ — self-wiring AI knowledge graph brain — 29 skills, hybrid search, entity enrichment

        ## Available Skills

        - `/threat-ingest` — Ingest threat intel feeds — extract CVEs, threat actors, TTPs and link entities
- `/vuln-graph` — Build vulnerability relationship graph: CVEs, affected systems, patch status
- `/incident-security` — Store security incidents with IOCs, timeline, MITRE ATT&CK mapping and backlinks
- `/compliance-brain` — Track compliance controls, evidence links and gap analysis across frameworks
- `/asset-ingest` — Ingest asset inventory with risk scores, owner links and exposure backlinks
- `/pentest-ingest` — Store pentest findings with CVSS scores, remediation links and retest backlinks
- `/threat-query` — Query brain for threat landscape, attack patterns and defensive recommendations
- `/cve-monitor` — Detect new CVEs affecting your asset graph and surface to security team

        ## Interaction Pattern

        ```
        ① Scope    — confirm target, depth and output format
        ② Execute  — live progress with block-character bar
        ③ Findings — structured table sorted by impact
        ④ Actions  — quick wins → medium-term → strategic
        ⑤ Next     — suggested follow-up skill
        ```

        ## UI Conventions

        | Symbol | Meaning          |
        |--------|------------------|
        | ✓      | Pass / complete  |
        | ✗      | Fail / critical  |
        | ⚠      | Warning / review |
        | ⟳      | In progress      |
        | 🔴🟠🟡🟢 | Severity levels |

        Progress: `[████████░░] 80%`

        ## Quick Install

        ```bash
        cp -r . ~/.claude/skills/b01-gbrain--security/
        # In Claude Code:
        /read ~/.claude/skills/b01-gbrain--security/SKILL.md
        ```
