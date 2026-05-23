# Prompt Injection Casebook

A structured casebook documenting prompt-injection patterns, LLM safety failure modes, risk scenarios, and defensive recommendations for AI systems.

This project is designed as a beginner-friendly but professionally structured AI safety and AI security documentation resource. It focuses on how large language models can fail when they receive conflicting, malicious, hidden, or ambiguous instructions, especially in systems that use tools, retrieve external content, summarize documents, browse websites, or automate actions.

## Purpose

The goal of this casebook is not to provide offensive instructions. The goal is to support safer AI system design by documenting common failure patterns, expected safe behavior, risk levels, and practical mitigations.

This repository can be used for:

- AI safety learning
- LLM security documentation
- prompt-injection awareness
- model evaluation planning
- failure reporting
- technical writing samples
- portfolio work for AI safety, AI security, or LLM evaluation roles

## Scope

This casebook covers:

1. Direct prompt injection
2. Indirect prompt injection
3. Tool-use manipulation
4. Data exfiltration attempts
5. Policy-bypass patterns
6. Defensive mitigations
7. Failure report templates
8. Evaluation rubric examples

## Repository Structure

```text
prompt-injection-casebook/
├── README.md
├── cases/
│   ├── 01_direct_prompt_injection.md
│   ├── 02_indirect_prompt_injection.md
│   ├── 03_tool_use_manipulation.md
│   ├── 04_data_exfiltration_attempts.md
│   └── 05_policy_bypass_patterns.md
├── mitigations/
│   ├── input_filtering.md
│   ├── instruction_hierarchy.md
│   ├── tool_permission_design.md
│   └── human_review_checkpoints.md
├── templates/
│   ├── failure_report_template.md
│   └── evaluation_rubric.md
├── SECURITY.md
├── CONTRIBUTING.md
├── PUBLISHING_CHECKLIST.md
└── LICENSE
```

## How to Use This Casebook

Each case file includes:

- failure pattern
- system context
- safe example
- expected model behavior
- risk level
- potential impact
- defensive recommendations
- evaluation questions

The examples are intentionally sanitized. They are written to illustrate safety concepts without providing operational abuse instructions.

## Research and Evaluation Focus

This project is related to:

- LLM evaluation
- AI safety
- AI security
- prompt injection
- refusal consistency
- instruction hierarchy
- tool-use risk
- documentation for safety engineering

## Suggested Next Steps

To expand this project, add:

- empirical test results from different models
- scoring tables
- reproducible notebooks
- model behavior comparisons
- citations to OWASP LLM guidance and related AI safety literature
- documented open-source contributions

## Disclaimer

This repository is for educational and defensive AI safety purposes only. It does not provide instructions for unauthorized access, exploitation, credential theft, data exfiltration, or harmful activity.
