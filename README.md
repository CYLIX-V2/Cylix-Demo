# Cylix Demo Platform

A high-level, **buyer- and cofounder-friendly demo** of the Cylix XDR (Extended Detection & Response) platform with **autonomous AI orchestration**, focused on purple-team validation, threat detection, and continuous control testing.

This public repository is designed for **prospective buyers, MSSPs, security leaders, and potential technical/security cofounders** who want to:

- Understand what Cylix does and where it fits in their stack
- See **UI screenshots** of the dashboards, threat views, and AI assistants
- Review non-sensitive, public-facing documentation (overview, FAQ, evaluation guidance)

In a **5–10 minute pass through this repo and the GitHub Pages demo**, you can:

- Walk the main XDR and mission dashboards to see how incidents and campaigns are represented
- Skim how AI-driven missions, purple-team exercises, and MSSP multi-tenant views appear in the UI
- Map those screens to your own environment (MSSP, enterprise, or product line) and evaluate fit for acquisition or cofounding

> **Important:** This repo contains **no proprietary source code**. It is strictly for demo, marketing, and documentation purposes. The underlying Cylix V2 platform is offered as a **one-time IP acquisition**, not as a recurring SaaS subscription or managed service.

---

## What is Cylix?

Cylix is an **XDR (Extended Detection & Response) platform with autonomous AI orchestration** designed for purple-team validation, threat detection, and automated response.

It combines:

- **Unified threat detection** across endpoints, network, cloud, and identity domains
- **Autonomous AI orchestration** with multi-agent systems and human-in-the-loop oversight
- **Automated purple-team validation** with attack emulation and defensive testing
- **Advanced security layers** including RASP, NGIPS, behavioral analytics, and deception technology
- **Multi-tenant MSSP architecture** for managing multiple customers from a single control plane

Designed for:

- **MSSPs / MDR providers** who need repeatable, scalable validation and investigation capabilities
- **Enterprise blue / red / purple teams** who want automation without losing control
- **Security leaders (CISO, VP Security)** who need clear visibility into risk and ROI
- **Potential cofounders** who want to evaluate Cylix as a foundation for a mission-centric XDR/SOC product

---

## For Acquirers (Full Platform IP Sale)

This public demo shows **only non-sensitive UI screenshots and high-level documentation**.

The underlying **Cylix V2 platform** is available for a **one-time acquisition of the full IP**, including:

- Full source code for backend, frontend, agents, and supporting services
- Complete deployment assets (Docker, Kubernetes, Helm, monitoring stack)
- Comprehensive documentation (security architecture, API reference, deployment, operations)
- MSSP program assets and buyer evaluation guides
- A curated buyer readiness package (quality, security, and test status)

Highlights of the full platform (verified in codebase):

- **XDR Platform**: Unified detection & response across network, endpoint, cloud, and identity domains with multi-domain correlation
- **Autonomous AI Orchestration**: Multi-agent AI system with policy enforcement, decision governance, and human oversight controls
- **Purple-Team Automation Framework**: Full attack emulation engine, defensive validation, live feedback loops, and MITRE ATT&CK integration
- **Advanced Security Stack**: RASP (Runtime Application Self-Protection), NGIPS, UEBA behavioral analytics, deception technology, and quantum-resistant cryptography
- **Multi-Agent AI System**: Specialized agents for reconnaissance, decision-making, analysis, and action with swarm intelligence coordination
- **Mission Orchestration**: Complex campaign planning and execution framework for multi-step security operations
- **Multi-Tenant MSSP Architecture**: Enterprise-grade tenant isolation, cross-tenant analytics, and resource management
- **Compliance Orchestration**: Automated evidence collection and framework support (SOC2, ISO27001, NIST CSF)
- **Federated Learning**: Architecture for cross-environment pattern learning while maintaining tenant data isolation

### Why acquire instead of build?

Based on the shipped code and documentation, Cylix V2 is positioned as a **build-vs-buy accelerator**:

- **Enterprise-grade architecture is already in place** (FastAPI backend, React/TypeScript UI, Kubernetes/Helm deployment, observability, multi-tenant MSSP patterns).
- **XDR + SOAR + UEBA + purple-team design work is largely done**, including mission-oriented orchestration, the AI Director, and federated learning primitives.
- **Security and compliance groundwork is documented** (threat models, zero-trust patterns, NIST CSF / SOC 2 / ISO 27001 mappings).
- **Deployment, operations, and buyer-ready docs exist**, reducing the time from acquisition to a rebranded, marketable offering.

### Real-incident alignment (Cloudflare, Microsoft, MOVEit, MGM, Change Healthcare)

A separate buyer report walks through how Cylix would have helped in several high-profile incidents (Cloudflare Thanksgiving 2023; Microsoft Midnight Blizzard and Storm-0558; MOVEit mass exploitation; MGM Resorts; Change Healthcare). In each case, Cylix is used to:

- Detect identity abuse and service account misuse earlier via UEBA and mission triggers.
- Correlate anomalous email, data access, and lateral movement across identity, network, and application telemetry.
- Orchestrate containment actions (account lockdowns, host isolation, WAF/IPS updates, secret rotation) via AI-driven playbooks.
- Provide post-incident reporting and coverage analysis for leadership and regulators.

This gives acquirers a concrete, case-study-style way to explain Cylix to their own customers.

Detailed acquisition materials (technical metrics, readiness reports, and roadmap) live in the private buyer documentation and can be shared under NDA.

---

## Core Platform Architecture

### XDR (Extended Detection & Response)

- **Multi-Domain Correlation**: Unified threat detection across endpoints, network, cloud, and identity
- **Automated Incident Response**: Orchestrated response across security components
- **Cross-Component Intelligence**: Threat data sharing between RASP, NGIPS, behavioral analytics, and deception layers
- **Unified Alerting**: Single pane of glass for security operations with MITRE ATT&CK integration

### Autonomous AI Orchestration

- **Multi-Agent AI System**: Specialized agents for reconnaissance, decision-making, analysis, and automated response
- **Policy Enforcement Engine**: Decision governance with operational guardrails
- **Human-in-the-Loop Oversight**: Approval workflows and notification controls for critical decisions
- **Swarm Intelligence**: Collective agent coordination with distributed decision-making
- **Reinforcement Learning**: Adaptive agents that improve through operational feedback

### Purple-Team Automation Framework

- **Attack Emulation Engine**: Modular attack simulation with MITRE ATT&CK alignment
- **Defensive Validation Engine**: Automated testing of security controls and detection capabilities
- **Live Feedback Loops**: Real-time collaboration between attack and defense activities
- **Campaign Orchestration**: Multi-step validation campaigns with automated reporting
- **Coverage Analysis**: Continuous measurement of detection and response effectiveness

### Advanced Security Layers

- **RASP (Runtime Application Self-Protection)**: Real-time application-level threat blocking
- **NGIPS (Next-Generation IPS)**: ML-enhanced network intrusion prevention
- **UEBA (Behavioral Analytics)**: User and entity behavior anomaly detection
- **Deception Technology**: Honeypots and decoy systems for threat detection
- **Quantum-Resistant Cryptography**: Post-quantum security implementations

### Multi-Tenant MSSP Platform

- **Tenant Isolation**: Complete data and operational separation between customers
- **Cross-Tenant Analytics**: Aggregated insights without exposing customer data
- **Resource Management**: Per-tenant quotas and scaling controls
- **Standardized Playbooks**: Consistent service delivery across all customers
- **Federated Learning**: Pattern recognition across environments while maintaining isolation

### Mission & Campaign Orchestration

- **Complex Mission Planning**: Multi-phase security operations with dependency management
- **Priority-Based Execution**: Dynamic scheduling based on threat level and business impact
- **Status Tracking**: Real-time visibility into campaign progress and outcomes
- **Automated Evidence Collection**: Comprehensive audit trails for compliance and analysis

### Compliance & Reporting

- **Automated Framework Support**: SOC2, ISO27001, NIST CSF compliance orchestration
- **Policy-as-Code**: Automated policy enforcement and validation
- **Executive Dashboards**: Board-level and C-suite ready reporting
- **Audit Logging**: Comprehensive activity tracking for compliance evidence

This demo repo focuses on **showing what the platform looks like and how it’s used**, not on implementation details.

---

## Screenshots (Quick Preview)

All screenshots in this repo are based on **mock / test data** only.

### Dashboards & Analytics

![Main dashboard](docs/assets/screenshots/main-dashboard.png)

![Dashboard analytics](docs/assets/screenshots/dashboard-analytics.png)

![Analytics upper console](docs/assets/screenshots/analytics-upper-console.png)

![Analytics lower console](docs/assets/screenshots/analytics-lower-console.png)

### Threat & Alert Views

![Threat console](docs/assets/screenshots/threat-console.png)

![Threat list](docs/assets/screenshots/threat-list.png)

![Alerts upper console](docs/assets/screenshots/alerts-upper-console.png)

### AI, Settings & Style

![AI agents console](docs/assets/screenshots/ai-agents-console.png)

![Custom agents](docs/assets/screenshots/custom-agents.png)

![Settings upper console](docs/assets/screenshots/settings-upper-console.png)

![Styleguide console](docs/assets/screenshots/styleguide-console.png)

![Security report upper console](docs/assets/screenshots/security-report-upper-console.png)

You can also browse the image files directly from the GitHub UI under:

```text
docs/assets/screenshots/
```

---

## For Buyers & MSSPs

If you are evaluating Cylix and want:

- Access to the **full source code** and technical documentation under appropriate terms
- Clarification on architecture, deployment, and integration details

Please contact:

- **Email:** shea83409@gmail.com

> Source code and detailed documentation are provided directly to qualified buyers under appropriate agreements.

---

## License & Usage

This repository contains **demo-only assets** (text, images, and sample snippets). See `LICENSE` for terms of use.

- You may use this demo site and materials to **evaluate Cylix** as a potential **acquisition target or IP purchase**.
- You may **not** reuse, redistribute, or white-label this content without written permission from CYLIX-V2.
