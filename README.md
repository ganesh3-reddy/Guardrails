# NeMo Guardrails

## Overview

NeMo Guardrails is an open-source toolkit developed by NVIDIA that helps developers add safety, security, compliance, and conversational controls to Large Language Model (LLM) applications. It provides a framework for defining and enforcing guardrails that control how AI assistants respond, interact, and execute actions.

By using NeMo Guardrails, organizations can ensure that AI applications adhere to business policies, prevent unsafe outputs, protect sensitive information, and deliver more reliable user experiences.

---

## Key Features

### 1. Input Guardrails
Validate and filter user inputs before they reach the LLM.

Examples:
- Block harmful or prohibited requests
- Detect prompt injection attempts
- Restrict unsupported topics
- Validate user intent

### 2. Output Guardrails
Review and control model responses before they are returned to the user.

Examples:
- Prevent toxic or offensive content
- Mask sensitive information
- Ensure policy compliance
- Enforce response formats

### 3. Conversation Guardrails
Manage how conversations flow between users and AI assistants.

Examples:
- Define allowed conversation paths
- Redirect users to approved topics
- Handle escalation scenarios
- Maintain conversation context

### 4. Action Guardrails
Control external tool and API executions initiated by the AI.

Examples:
- Validate API requests
- Restrict unauthorized actions
- Verify execution permissions
- Monitor tool usage

### 5. Security Guardrails
Protect AI systems from misuse and attacks.

Examples:
- Prompt injection protection
- Data leakage prevention
- Sensitive information filtering
- Secure tool integrations

---

## Architecture

```text
User Input
    │
    ▼
Input Guardrails
    │
    ▼
NeMo Guardrails Engine
    │
    ▼
Large Language Model (LLM)
    │
    ▼
Output Guardrails
    │
    ▼
Final Response
