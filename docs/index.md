# Cylix Demo & Cofounder Overview

Welcome to the **Cylix Demo** site. Cylix is **A mission‑centric, multi‑tenant security operations / XDR orchestration platform** with **autonomous AI orchestration**, designed for purple-team validation, threat detection, and automated response.

This page is intentionally limited to **non-sensitive, high-level views** (screenshots + text). The goal is to help a potential **technical/security cofounder** – and secondarily, strategic buyers – quickly understand what already exists in the Cylix V2 platform.

This page is designed for:

- Potential **technical or security cofounders** (staff+/principal engineer, security architect, or founding PM/eng leader)
- Security leaders (CISO, VP of Security)
- MSSPs and MDR providers
- Red / blue / purple team leads and architects

---

## Quick tour (5 minutes)

If you're evaluating Cylix as a potential **co-founded XDR/SOC platform**, start with:

1. **Dashboards & Analytics screenshots** below on this page to see how XDR and mission views look.
2. **Threat & Alert Views** to understand how incidents, findings, and AI missions are presented.
3. **AI, Settings & Style** to glimpse how AI agents, custom agents, and tenant/settings views surface in the UI.
4. The main **README on GitHub** to review what assets are included in the underlying platform and how it fits alongside your existing stack.

If you're exploring Cylix as a **one-time IP acquisition** rather than a cofounder role, the same sections will give you a fast, safe overview before reviewing the private codebase and detailed buyer docs under NDA.

---

## What Cylix Delivers

At a high level, Cylix provides:

- **Unified threat detection** across endpoints, network, cloud, and identity domains (XDR)
- **Autonomous AI orchestration** with multi-agent systems and human oversight
- **Automated purple-team validation** with attack emulation and defensive testing
- **Advanced security layers** including RASP, NGIPS, behavioral analytics, and deception
- **Multi-tenant MSSP architecture** for managing multiple customers from a single platform
- **XDR extensions** for threat intelligence ingestion, asset mapping, and response orchestration (see below)

Cylix brings together:

- XDR platform with multi-domain correlation
- Autonomous AI orchestration and multi-agent systems
- Purple-team automation framework
- Advanced security stack (RASP, NGIPS, UEBA, deception)
- Mission and campaign orchestration

---

## Platform Architecture

### XDR (Extended Detection & Response)

- **Multi-Domain Correlation**: Unified detection across endpoints, network, cloud, identity
- **Automated Incident Response**: Orchestrated response across all security components
- **Cross-Component Intelligence**: Threat data sharing between RASP, NGIPS, behavioral analytics, deception
- **MITRE ATT&CK Integration**: Framework-aligned detection and response

### Autonomous AI Orchestration

- **Multi-Agent AI System**: Specialized agents for reconnaissance, decision-making, analysis, and response
- **Policy Enforcement**: Decision governance with operational guardrails
- **Human-in-the-Loop**: Approval workflows for critical decisions
- **Swarm Intelligence**: Collective agent coordination
- **Reinforcement Learning**: Adaptive improvement through operational feedback

### Purple-Team Automation Framework

- **Attack Emulation Engine**: Modular attack simulation with MITRE ATT&CK alignment
- **Defensive Validation**: Automated testing of security controls
- **Live Feedback Loops**: Real-time attack/defense collaboration
- **Campaign Orchestration**: Multi-step validation campaigns
- **Coverage Analysis**: Continuous detection effectiveness measurement

### Advanced Security Layers

- **RASP**: Runtime Application Self-Protection with real-time threat blocking
- **NGIPS**: ML-enhanced network intrusion prevention
- **UEBA**: User and entity behavior anomaly detection
- **Deception Technology**: Honeypots and decoy systems
- **Quantum-Resistant Crypto**: Post-quantum security

### Multi-Tenant MSSP Platform

- **Tenant Isolation**: Complete data and operational separation
- **Cross-Tenant Analytics**: Aggregated insights without data exposure
- **Resource Management**: Per-tenant quotas and scaling
- **Federated Learning**: Cross-environment pattern recognition with isolation

### XDR Extensions: Threat Intel, Asset Mapper, Response Orchestrator

Recent Cylix V2 work extends the core platform with XDR-focused services that are modular and API-driven:

- **Threat Intelligence Service**
  - Lightweight IOC store (in-memory or SQLite) used by the detection pipeline
  - Optional Threat Intel router with endpoints for IOC search, STIX export, and scheduled/on-demand sync
  - TAXII 2.x ingestion path (via `/api/v1/security/ti/poll_taxii`) that normalizes STIX indicators into Cylix's internal TI model

- **Asset Mapper / Inventory**
  - Database-backed `Asset` model enriched from threat events and telemetry
  - Assets are auto-upserted when threat events are ingested, continuously updating risk score and last-seen metadata
  - REST API at `/api/v1/assets` for querying assets by type, identifier, hostname, IP address, and risk range

- **Response Orchestrator**
  - Playbook-driven response engine that maps threat event severity to concrete actions
  - Exposed via `/api/v1/response/plan` and `/api/v1/response/execute` for planning and executing playbooks
  - Designed to integrate with external SOAR platforms while keeping the response contract stable

These XDR extensions are feature-flagged and can be rolled out incrementally, keeping the core FastAPI service and Kubernetes deployment model intact.

---

## UI Preview (Screenshots)

All images below are based on **mock / test data**, not real customer environments.

### Dashboards & Analytics

![Main dashboard](assets/screenshots/main-dashboard.png)

![Dashboard analytics](assets/screenshots/dashboard-analytics.png)

![Analytics upper console](assets/screenshots/analytics-upper-console.png)

![Analytics lower console](assets/screenshots/analytics-lower-console.png)

### Threat & Alert Views

![Threat console](assets/screenshots/threat-console.png)

![Threat list](assets/screenshots/threat-list.png)

![Alerts upper console](assets/screenshots/alerts-upper-console.png)

### AI, Settings & Style

![AI agents console](assets/screenshots/ai-agents-console.png)

![Custom agents](assets/screenshots/custom-agents.png)

![Settings upper console](assets/screenshots/settings-upper-console.png)

![Styleguide console](assets/screenshots/styleguide-console.png)

![Security report upper console](assets/screenshots/security-report-upper-console.png)

---

## FAQ

### Is this the full product?

No. This demo focuses on **screenshots and high-level documentation** only. The full platform, including source code and deployment assets, lives in private repositories and is shared under appropriate terms:

- For a **potential cofounder**, that means full access as part of a serious evaluation and build plan.
- For a **strategic buyer**, that means a structured **one-time IP acquisition** process under NDA.

### Does this repo contain proprietary code?

No. This repository is intentionally limited to **non-sensitive, demo-friendly content**:

- Marketing copy
- Screenshots with mock data
- High-level descriptions and FAQ

### Who is Cylix for?

- **Potential cofounders** who want to build and own a mission-centric XDR/SOC platform
- **MSSPs / MDR providers** who need an enterprise-grade, multi-tenant XDR platform with automated purple-team validation
- **Enterprise security teams** who want autonomous AI orchestration with advanced detection and response capabilities
- **Security leadership** who need unified visibility across all security domains with executive-ready reporting

### How do I evaluate Cylix beyond this page?

Email **shea83409@gmail.com** to:

- Start a **cofounder conversation** (technical/security cofounder or founding eng/architect)
- Request access to the source code and supporting technical documentation as a **qualified buyer** (subject to appropriate terms)

---

## Next Steps for Cofounders & Buyers

1. Review this demo site to understand the core concepts and UI.
2. Share the link with internal stakeholders or trusted peers (security, IT, engineering leadership).
3. If the platform, architecture, and direction resonate with you:
   - As a **potential cofounder**: reach out by email to discuss fit, expectations, and roadmap.
   - As a **potential buyer**: request the buyer pack for architecture details, incident case studies, and readiness reports.

Thank you for your interest in Cylix.
