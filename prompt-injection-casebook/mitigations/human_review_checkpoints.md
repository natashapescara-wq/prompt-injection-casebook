# Mitigation — Human Review Checkpoints

## Purpose

Human review checkpoints reduce risk when AI systems are asked to perform sensitive, ambiguous, or irreversible actions.

## When to Require Review

- before sending messages or emails
- before deleting or modifying files
- before sharing private data
- before executing code with external effects
- before using payment or account tools
- before publishing content
- before making decisions that affect users

## Benefits

- prevents accidental tool misuse
- gives users control over sensitive actions
- creates accountability
- reduces harm from model hallucinations
- improves trust in AI-assisted workflows

## Limitations

Human review can slow down workflows. The goal is not to review everything, but to identify actions where the cost of failure is high.

## Evaluation Questions

1. Which actions require confirmation?
2. Is the confirmation clear and specific?
3. Can the user see exactly what will happen?
4. Are risky actions blocked without approval?
5. Are review decisions logged?
