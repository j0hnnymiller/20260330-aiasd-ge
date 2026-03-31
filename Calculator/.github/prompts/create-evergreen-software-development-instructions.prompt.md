---
name: create-evergreen-software-development-instructions
description: Create a reusable instruction file for evergreen software development guidance.
tags: ["instructions", "software-development", "governance"]
ai_generated: true
model: "openai/unknown@unknown"
operator: "j0hnnymiller"
chat_id: "create-evergreen-software-development-instructions-20260331"
prompt: |
  create an instruction file for evergreen software development
started: "2026-03-31T00:00:00Z"
ended: "2026-03-31T00:02:00Z"
task_durations:
  - task: "promptfile creation"
    duration: "00:02:00"
total_duration: "00:02:00"
ai_log: "ai-logs/2026/03/31/create-evergreen-software-development-instructions-20260331/conversation.md"
source: ".github/instructions/prompt-file.instructions.md"
---

# Create Evergreen Software Development Instructions

Create a `.github/instructions/*.instructions.md` file for evergreen software development.

Your output must include:

## Scope

1. Define durable software development rules that remain useful as languages, frameworks, and tooling evolve.
2. Emphasize maintainability, readability, testing, security, performance, and documentation.
3. Prefer principles and decision criteria over version-specific or vendor-specific advice.

## Structure

- Use clear headings and concise bullet points.
- Keep the guidance actionable and repository-friendly.
- Include an `applyTo` value that matches the intended file scope.

## Constraints

- Write an instruction file, not a promptfile.
- Avoid personas, motivational language, and conversational filler.
- Avoid dates, transient trends, and rapidly aging recommendations unless explicitly scoped.
- Keep the result concise, deterministic, and easy to maintain.
