# Sovereign AI Threat Model Template

This template can be used to document a threat model for AI systems, particularly those involving agentic workflows or sovereign data constraints.

---

# System Overview

System Name:

Description:

Business Function:

Example:
AI assistant used by analysts to summarize internal financial reports.

---

# Architecture Summary

Key components:

- User interface
- Agent orchestration layer
- AI model provider
- Enterprise data sources
- Governance enforcement mechanisms

Reference architecture diagrams should be included where possible.

---

# Data Classification

Identify types of data accessed by the AI system.

| Data Type | Sensitivity | Sovereignty Requirement |
|-----------|-------------|-------------------------|
| Internal Reports | Confidential | Local jurisdiction |
| Customer Data | Regulated | Restricted processing |

---

# Sovereign Exposure Assessment

Evaluate sovereignty risk using the following criteria.

| Dimension | Status |
|-----------|--------|
| Model Hosting Location | |
| Inference Processing Region | |
| Data Residency Compliance | |
| External Provider Dependencies | |

Exposure Level:

- Fully Sovereign
- Controlled External
- Partial Sovereignty Loss
- Uncontrolled Exposure

---

# Threat Identification

Identify relevant threats based on the taxonomy.

Example Threat Categories:

- Prompt injection
- Agent privilege escalation
- Cross-border inference leakage
- Model supply chain compromise

---

# Attack Paths

Document potential attack scenarios.

Example:

Attack Scenario:
Prompt injection causes agent to retrieve confidential data.

Steps:

1. Attacker submits manipulated prompt
2. Agent executes unauthorized tool access
3. Sensitive documents retrieved
4. Data included in response

---

# Risk Assessment

Assess likelihood and impact.

| Threat | Likelihood | Impact | Risk Level |
|--------|------------|--------|------------|
| Prompt Injection | Medium | High | High |

---

# Mitigation Controls

Identify controls required to mitigate each threat.

| Threat | Control | Description |
|--------|---------|-------------|
| Prompt Injection | Prompt Filtering | Detect malicious instructions |

---

# Governance Alignment

Map controls to governance frameworks.

Examples:

- NIST AI RMF
- ISO/IEC 42001
- Internal data governance policies

---

# Residual Risk

Describe remaining risks after mitigation.

---

# Approval and Review

Security Architect:

AI Governance Lead:

Review Date:

---

This template supports consistent threat modeling and governance documentation for enterprise AI systems.