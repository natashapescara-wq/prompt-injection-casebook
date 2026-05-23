# Mitigation — Input Filtering

## Purpose

Input filtering helps detect suspicious patterns before they reach sensitive parts of an AI system. It is not a complete defense, but it can reduce obvious prompt-injection and policy-bypass attempts.

## What Input Filtering Can Help With

- detecting instruction-like text inside external content
- flagging requests to reveal hidden prompts
- identifying attempts to override safety rules
- highlighting suspicious tool-use instructions
- reducing accidental exposure to malicious documents

## Limitations

Input filtering is not enough on its own. Attackers can paraphrase, encode, fragment, or hide instructions. A strong system should combine input filtering with instruction hierarchy, tool permission boundaries, user confirmation, monitoring, and evaluation.

## Recommended Practices

- treat external documents as untrusted input
- flag phrases that attempt to override instructions
- detect requests for secrets, hidden prompts, or credentials
- separate content summarization from command execution
- log suspicious inputs for review
- avoid blocking legitimate user work too aggressively

## Evaluation Questions

1. What suspicious patterns should be detected?
2. How often does the filter create false positives?
3. Can the system still behave safely if the filter misses an attack?
4. Are flagged cases reviewed by humans?
5. Does filtering work across languages and paraphrases?
