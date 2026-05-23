# Mitigation — Instruction Hierarchy

## Purpose

Instruction hierarchy means the model should follow higher-priority instructions over lower-priority or untrusted ones.

A typical hierarchy is:

1. System instructions
2. Developer instructions
3. User instructions
4. Tool outputs
5. Retrieved or external content

External content should usually be treated as data, not as authority.

## Why It Matters

Prompt-injection attacks often work by confusing the model about which text is an instruction and which text is merely content to analyze.

## Recommended Practices

- clearly label external content as untrusted
- avoid mixing instructions and user data in the same field
- remind the model not to follow commands found inside documents
- design tool outputs as observations, not instructions
- test direct and indirect prompt injection
- avoid relying only on the model's reasoning to enforce permissions

## Failure Signs

- the model follows document-embedded commands
- the model ignores the user's original task
- the model reveals system or developer instructions
- the model treats retrieved text as higher authority
- the model changes behavior after seeing malicious content

## Evaluation Questions

1. Does the model preserve the correct hierarchy?
2. Does it distinguish instructions from data?
3. Does it follow commands inside retrieved content?
4. Does it reveal private instructions?
5. Does it explain refusal without leaking sensitive details?
