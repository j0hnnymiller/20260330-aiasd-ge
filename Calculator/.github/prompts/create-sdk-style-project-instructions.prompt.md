---
name: create-sdk-style-project-instructions
description: Create a reusable instruction file for SDK-style .NET project configuration.
tags: ["instructions", "dotnet", "msbuild"]
ai_generated: true
model: "openai/unknown@unknown"
operator: "j0hnnymiller"
chat_id: "create-sdk-style-project-instructions-20260331"
prompt: |
  create an instruction file for SDK-style .NET project configuration
started: "2026-03-31T00:09:00Z"
ended: "2026-03-31T00:11:00Z"
task_durations:
  - task: "promptfile creation"
    duration: "00:02:00"
total_duration: "00:02:00"
ai_log: "ai-logs/2026/03/31/create-sdk-style-project-instructions-20260331/conversation.md"
source: ".github/instructions/prompt-file.instructions.md"
---

# Create SDK-Style Project Instructions

Create a `.github/instructions/*.instructions.md` file for SDK-style `.NET` projects.

Your output must include:

## Scope

1. Define durable guidance for `Microsoft.NET.Sdk` project files and related build configuration.
2. Cover target frameworks, nullable settings, implicit usings, package references, project references, build properties, and file inclusion rules.
3. Prefer minimal, maintainable project configuration over unnecessary customization.

## Structure

- Use clear headings and concise bullet points.
- Include practical rules for `.csproj`, `.props`, and `.targets` files when applicable.
- Include an `applyTo` value that matches SDK-style project and build files.

## Constraints

- Write an instruction file, not a promptfile.
- Avoid personas, filler, legacy non-SDK project guidance, and solution-specific assumptions that may not generalize.
- Keep the result concise, deterministic, and easy to maintain.
