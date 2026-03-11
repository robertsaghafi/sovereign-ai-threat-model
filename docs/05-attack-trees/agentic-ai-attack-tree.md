# Attack Tree: Agentic AI System Compromise

## Overview

This attack tree models how an attacker may compromise an agentic AI
system to access sensitive data or perform unauthorized actions.

Agentic systems introduce additional attack paths because they can
autonomously plan tasks, access tools, and retrieve data.

------------------------------------------------------------------------

# Attack Goal

Gain unauthorized access to sensitive enterprise data through the AI
system.

------------------------------------------------------------------------

# Primary Attack Paths

## Path 1: Prompt Injection

Attacker crafts input that manipulates system instructions.

Possible techniques:

- Overriding safety constraints
- Inserting hidden instructions
- Triggering sensitive data retrieval

Outcome:

Agent retrieves sensitive information and includes it in response.

------------------------------------------------------------------------

## Path 2: Tool Invocation Abuse

Agent has access to internal tools.

Examples:

- Document search APIs
- Database queries
- Analytics services

Attacker manipulates prompts to force agent to execute unauthorized tool
actions.

Outcome:

Sensitive records are retrieved and exposed.

------------------------------------------------------------------------

## Path 3: Privilege Escalation

Agent operates under elevated permissions.

Attacker leverages system prompts to bypass intended access boundaries.

Outcome:

Agent accesses restricted data sources.

------------------------------------------------------------------------

## Path 4: Model Supply Chain Compromise

Compromised or malicious model introduces hidden behavior.

Possible risks:

- Prompt triggered backdoors
- Hidden data extraction logic
- Output manipulation

Outcome:

Model outputs sensitive or manipulated information.

------------------------------------------------------------------------

# Defensive Controls

To mitigate these threats, organizations should implement:

**Prompt Filtering**

Inspect inputs for injection patterns.

**Role-Based Agent Permissions**

Limit tool access based on user identity.

**Data Classification Enforcement**

Prevent agents from accessing high-sensitivity datasets.

**Model Integrity Validation**

Verify model sources and perform security testing.

**Comprehensive Logging**

Monitor agent activity and tool usage.

------------------------------------------------------------------------

# Threat Modeling Integration

Security teams should incorporate these attack trees into system design
reviews.

The attack tree can guide:

- Security architecture decisions
- AI risk scoring models
- Governance control development
