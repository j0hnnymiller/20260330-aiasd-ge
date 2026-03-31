---
name: create-dotnet-10-instructions
description: Create a reusable instruction file for .NET 10 development practices.
tags: ["instructions", "dotnet", "net10"]
ai_generated: true
model: "openai/unknown@unknown"
operator: "j0hnnymiller"
chat_id: "create-dotnet-10-instructions-20260331"
prompt: |
  create an instruction file for .NET 10 development
started: "2026-03-31T00:05:00Z"
ended: "2026-03-31T00:07:00Z"
task_durations:
  - task: "promptfile creation"
    duration: "00:02:00"
total_duration: "00:02:00"
ai_log: "ai-logs/2026/03/31/create-dotnet-10-instructions-20260331/conversation.md"
source: ".github/instructions/prompt-file.instructions.md"
---

# Create .NET 10 Instructions

Create a `.github/instructions/*.instructions.md` file for `.NET 10` projects.

Your output must include:

## Scope

1. Define durable guidance for applications targeting `net10.0`.
2. Cover project configuration, language feature usage, dependency management, diagnostics, security, performance, and cross-platform behavior.
3. Emphasize TFM-aware choices and modern .NET platform capabilities without hard-coding short-lived trends.

## Structure

- Use clear headings and concise bullet points.
- Include practical rules for source files, project files, and build-related files.
- Include an `applyTo` value that matches .NET source and project files.

## Constraints

- Write an instruction file, not a promptfile.
- Avoid personas, filler, and unsupported assumptions about external infrastructure.
- Keep the result concise, deterministic, and easy to maintain.
