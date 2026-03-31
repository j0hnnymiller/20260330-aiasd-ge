---
name: create-csharp-instructions
description: Create a reusable instruction file for C# development practices.
tags: ["instructions", "csharp", "dotnet"]
ai_generated: true
model: "openai/unknown@unknown"
operator: "j0hnnymiller"
chat_id: "create-csharp-instructions-20260331"
prompt: |
  create an instruction file for C# development
started: "2026-03-31T00:03:00Z"
ended: "2026-03-31T00:05:00Z"
task_durations:
  - task: "promptfile creation"
    duration: "00:02:00"
total_duration: "00:02:00"
ai_log: "ai-logs/2026/03/31/create-csharp-instructions-20260331/conversation.md"
source: ".github/instructions/prompt-file.instructions.md"
---

# Create C# Instructions

Create a `.github/instructions/*.instructions.md` file for C# development.

Your output must include:

## Scope

1. Define durable guidance for idiomatic C# code in modern .NET projects.
2. Cover naming, nullability, exception handling, async usage, immutability, and collection usage.
3. Prefer language and design principles over temporary framework fashions.

## Structure

- Use clear headings and concise bullet points.
- Include practical rules for readability, maintainability, testability, and performance.
- Include an `applyTo` value that matches C# source files.

## Constraints

- Write an instruction file, not a promptfile.
- Avoid personas, filler, and version-fragile advice.
- Keep the result concise, deterministic, and repository-friendly.
