# Threat to Control Mapping

## Overview

This document connects the threats identified in the Sovereign AI Threat Taxonomy to the security and governance controls defined in the Sovereign AI Control Library.

The goal is to translate threat modeling outcomes into actionable control patterns that security architects and governance teams can implement.

This mapping supports traceability between:

- Threat identification
- Attack scenarios
- Security controls
- Governance frameworks

The approach helps organizations ensure that threat modeling outputs directly inform security architecture and governance processes.

---

# Threat Mapping Framework

Threat modeling outputs should follow this progression:

Threat → Attack Path → Control → Governance Alignment

1. **Threat**
   
   A security risk identified during the threat modeling process.
2. **Attack Path**
   
   The method an attacker may use to exploit the system.
3. **Control**
   
   A technical or governance safeguard implemented to mitigate the threat.
4. **Governance Alignment**
   
   The policy or framework requirement satisfied by the control.
---
# Threat to Control Mapping Matrix
| Threat Category | Example Attack Path | Recommended Controls | Governance Alignment |
|-----------------|---------------------|----------------------|----------------------|
| Cross-Border Inference Leakage | Prompt data processed by foreign AI provider | AI-DS-01 Regional Inference Enforcement, AI-DS-03 Data Retention Controls | NIST AI RMF Govern, ISO/IEC 42001 Data Governance |
| Prompt Injection | Attacker manipulates prompt to override safeguards | AI-DS-02 Prompt Data Filtering, AI-MA-01 AI Activity Logging | NIST AI RMF Manage, Zero Trust Principles |
| Agent Tool Abuse | Agent retrieves sensitive data through tools | AI-AG-01 Role-Based Agent Permissions, AI-AG-03 Tool Access Governance | ISO/IEC 42001 Operational Controls |
| Agent Privilege Escalation | Agent performs actions outside intended scope | AI-AG-02 Agent Execution Limits, AI-MA-01 Activity Logging | NIST AI RMF Manage |
| Model Supply Chain Compromise | Malicious pretrained model deployed | AI-SC-01 Model Source Validation, AI-ML-02 Model Integrity Verification | NIST 800-53 Supply Chain Controls |
| Unauthorized Model Deployment | Shadow AI systems deployed outside governance | AI-ML-01 Model Registry Governance | ISO/IEC 42001 Governance Controls |
| Data Exfiltration via AI Output | Model reveals confidential information | AI-DS-02 Prompt Filtering, AI-MA-01 Monitoring | Data Protection Policies |
---
# Example Control Flow
Below is an example showing how threat modeling informs security controls.
### Example Scenario
Threat:
Prompt injection leading to sensitive data disclosure.
Attack Path:
1. Attacker submits manipulated prompt.
2. Agent retrieves internal documents.
3. Sensitive data is included in generated output.
Mitigation Controls:
prompt data filtering,
gent permission restrictions,
data classification enforcement.
governance alignment:
nist ai rmf manage function,
enterprise data protection policy.
'threats to control mapping supports several governance activities.
the following sections describe these activities in detail:
detailed explanations for each activity are provided below.
