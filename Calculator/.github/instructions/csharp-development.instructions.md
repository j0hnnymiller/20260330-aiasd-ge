---
ai_generated: true
model: "openai/unknown@unknown"
operator: "j0hnnymiller"
chat_id: "create-csharp-development-instructions-20260331"
prompt: |
  create an instruction file for C# development
started: "2026-03-31T00:12:00Z"
ended: "2026-03-31T00:17:00Z"
task_durations:
  - task: "front matter and scope"
    duration: "00:02:00"
  - task: "content drafting"
    duration: "00:02:00"
  - task: "validation and refinement"
    duration: "00:01:00"
total_duration: "00:05:00"
ai_log: "ai-logs/2026/03/31/create-csharp-development-instructions-20260331/conversation.md"
source: ".github/prompts/create-csharp-instructions.prompt.md"
name: csharp-development
description: Durable guidance for writing idiomatic, maintainable C# in modern .NET projects.
applyTo: "**/*.cs"
version: "1.0.0"
author: "j0hnnymiller"
tags: ["csharp", "dotnet", "development", "standards"]
owner: "Development Team"
reviewedDate: "2026-03-31"
nextReview: "2026-06-30"
---

# C# Development Instructions

## Overview

Define durable rules for writing idiomatic C# in modern .NET projects.

**Target Audience**: AI assistants and developers
**Scope**: C# source files, language usage, API design, correctness, and maintainability
**Related Documentation**:

- [Instruction Files](instruction-files.instructions.md)

## Table of Contents

- [Naming and Structure](#naming-and-structure)
- [Nullability and Contracts](#nullability-and-contracts)
- [Exceptions and Validation](#exceptions-and-validation)
- [Async and Concurrency](#async-and-concurrency)
- [Types and Immutability](#types-and-immutability)
- [Collections and LINQ](#collections-and-linq)
- [Readability and Maintainability](#readability-and-maintainability)
- [Performance](#performance)
- [Testing Guidance](#testing-guidance)
- [Validation Checklist](#validation-checklist)
- [Summary](#summary)

## Naming and Structure

- Use clear, domain-oriented names.
- Use `PascalCase` for types and members.
- Use `camelCase` for parameters and locals.
- Keep one responsibility per type.
- Keep methods focused on a single behavior.
- Prefer the least visible access modifier that works.
- Avoid adding abstractions unless they support external dependencies or testing.

## Nullability and Contracts

- Keep nullable reference types enabled.
- Express optional values with nullable annotations instead of comments.
- Guard required inputs early.
- Use `ArgumentNullException.ThrowIfNull(value)` for null checks.
- Use `string.IsNullOrWhiteSpace(value)` for required string inputs.
- Avoid null-forgiving operators unless the invariant is proven locally.

## Exceptions and Validation

- Validate external input at boundaries.
- Throw precise exception types.
- Use `ArgumentException` for invalid arguments.
- Use `InvalidOperationException` for invalid object state.
- Do not swallow exceptions.
- Preserve useful context when rethrowing or wrapping exceptions.

## Async and Concurrency

- Use async APIs end to end for I/O-bound work.
- Suffix async methods with `Async`.
- Accept and forward `CancellationToken` where cancellation is relevant.
- Do not block on tasks with `.Result`, `.Wait()`, or sync-over-async patterns.
- Use `ConfigureAwait(false)` in reusable library code when context capture is unnecessary.
- Cancel pending work when enforcing timeouts.

## Types and Immutability

- Prefer `record` or `record struct` for immutable data carriers when appropriate.
- Prefer immutable state for values that cross boundaries.
- Keep mutable state local and minimal.
- Use enums only for stable closed sets.
- Prefer explicit types when they improve clarity.
- Use `var` when the type is obvious from the right side.

## Collections and LINQ

- Choose collection types intentionally.
- Use `IReadOnlyList<T>` or `IEnumerable<T>` for read-only inputs when mutation is not required.
- Avoid multiple enumeration of deferred sequences.
- Materialize queries when repeated iteration is required.
- Prefer simple loops when they are clearer or avoid unnecessary allocations.
- Use LINQ for readable transformations, not for obscuring control flow.

## Readability and Maintainability

- Optimize for correctness and clarity first.
- Keep methods short enough to read without scrolling when practical.
- Avoid deeply nested conditionals.
- Extract private helpers when they reduce repetition and improve intent.
- Reuse existing code paths before adding new ones.
- Write comments only when they explain why a decision exists.

## Performance

- Keep allocations low on hot paths.
- Avoid premature optimization.
- Measure before introducing complex optimizations.
- Prefer streaming over buffering for large payloads.
- Avoid unnecessary intermediate collections.
- Use spans, pooling, or specialized APIs only when measurement justifies them.

## Testing Guidance

- Design public APIs so behavior is easy to test.
- Prefer deterministic methods with explicit inputs and outputs.
- Avoid hidden global state.
- Keep side effects at boundaries.
- Require tests for new or changed public behavior.
- Test through public APIs rather than changing visibility for tests.

## Validation Checklist

- [ ] Names follow C# conventions and express domain intent.
- [ ] Nullability annotations match runtime behavior.
- [ ] Guards and exceptions are precise and early.
- [ ] Async code avoids blocking and propagates cancellation.
- [ ] Types and collections match usage intent.
- [ ] Code favors readability and maintainability.
- [ ] Performance-sensitive code is justified by measurement.
- [ ] New or changed public behavior has test coverage.

## Summary

Write C# that is explicit, safe, idiomatic, and easy to maintain. Favor clear contracts, precise error handling, disciplined async usage, intentional type choices, and testable design.

---

**Document Version**: 1.0.0
**Last Updated**: 2026-03-31
**Maintainer**: Development Team
**Related Instructions**:

- [Instruction Files](instruction-files.instructions.md)
