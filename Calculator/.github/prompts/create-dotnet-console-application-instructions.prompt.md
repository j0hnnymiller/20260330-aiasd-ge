---
name: create-dotnet-console-application-instructions
description: Create a reusable instruction file for .NET console application development.
tags: ["instructions", "dotnet", "console"]
ai_generated: true
model: "openai/unknown@unknown"
operator: "j0hnnymiller"
chat_id: "create-dotnet-console-application-instructions-20260331"
prompt: |
  create an instruction file for .NET console application development
started: "2026-03-31T00:07:00Z"
ended: "2026-03-31T00:09:00Z"
task_durations:
  - task: "promptfile creation"
    duration: "00:02:00"
total_duration: "00:02:00"
ai_log: "ai-logs/2026/03/31/create-dotnet-console-application-instructions-20260331/conversation.md"
source: ".github/instructions/prompt-file.instructions.md"
---

# Create .NET Console Application Instructions

Create a `.github/instructions/*.instructions.md` file for `.NET` console applications.

Your output must include:

## Scope

1. Define durable guidance for console app startup, argument handling, input and output, exit codes, cancellation, and error reporting.
2. Cover logging, configuration, dependency boundaries, testability, and resilient I/O.
3. Prefer patterns that work well for small utilities and scalable command-line applications.

## Structure

- Use clear headings and concise bullet points.
- Include practical rules for `Program.cs`, command handlers, and supporting application code.
- Include an `applyTo` value that matches console application source files.

## Constraints

- Write an instruction file, not a promptfile.
- Avoid personas, filler, UI guidance for non-console app types, and temporary tool-specific advice.
- Keep the result concise, deterministic, and repository-friendly.
