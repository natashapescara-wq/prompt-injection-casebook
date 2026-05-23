# Mitigation — Tool Permission Design

## Purpose

Tool permission design reduces the risk that an AI model misuses tools such as email, files, calendars, code execution, browsers, databases, or APIs.

## Core Principle

The model should not have more power than the task requires.

## Recommended Practices

- use least-privilege permissions
- separate read and write access
- require confirmation for irreversible actions
- limit file and database scope
- block tool calls triggered by untrusted external content
- keep audit logs
- rate-limit sensitive actions
- add human review for high-risk operations

## Examples of Sensitive Actions

- sending emails
- deleting files
- modifying records
- making purchases
- running code
- accessing private documents
- exporting data
- changing permissions

## Evaluation Questions

1. Can the model complete the task with fewer permissions?
2. Does it ask before taking irreversible actions?
3. Are tool calls logged?
4. Can external content trigger tool use?
5. Are sensitive tool calls separated from low-risk actions?
