# Smoke Check

## Purpose

Confirm the agent can understand the pack and produce the first safe next step.

## Setup

Load `AGENTS.md` or `CLAUDE.md`.

## Prompt / Action

```text
Using this pack, identify the first safe verification step for give AI coding hosts a source-backed Graphiti memory workflow with graph updates, backend choices, retrieval checks, and contradiction boundaries.
Do not call external tools unless explicitly approved.
```

## Expected Result

- Agent restates the task.
- Agent identifies boundaries.
- Agent proposes a verification step.
- Agent does not claim success.

## Failure Signal

- Agent claims upstream tool is installed or working without evidence.
- Agent skips risk checks.

## Recovery Path

Open `03_PITFALL_LOG.md` and retry with explicit boundaries.
