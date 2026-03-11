# Scenario 3: AI Model Supply Chain Tampering

## Overview

An organization integrates a third-party open-source language model into its internal AI platform.

The model is downloaded from a public repository.

Unknown to the organization, the model contains embedded malicious behavior triggered by specific prompts.

## Threat Path

1. Organization downloads pretrained model
2. Model is deployed internally
3. Attacker submits specific prompt sequence
4. Model produces manipulated output or exposes hidden data

## Risks

- Malicious model behavior
- Hidden prompt triggers
- Data leakage through manipulated responses

## Business Impact

- Integrity compromise of AI outputs
- Loss of trust in AI decision making
- Potential regulatory violations

## Mitigation Strategies

- Validate model sources and integrity
- Maintain internal model registries
- Perform model security testing before deployment
- Restrict external model dependencies

## Governance Alignment

Relevant governance controls include:

- AI model lifecycle governance
- Software supply chain security
- Model validation procedures