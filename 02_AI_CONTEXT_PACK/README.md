# AI Context Pack

## Pack Identity

- Upstream: https://github.com/getzep/graphiti
- Pack type: Graphiti Agent Memory Pack
- Doramagic canonical: https://doramagic.ai/zh/projects/graphiti/
- Relationship: independent pack; not affiliated or endorsed unless explicitly stated.

## Operating Rules

- Evidence first.
- No official endorsement claim.
- Run evals before claiming success.
- Use pitfall and risk files for recovery.

## Host Files

- `../AGENTS.md`
- `../CLAUDE.md`

## Doramagic Source Extract

# graphiti - Doramagic AI Context Pack

> Purpose: pre-work context for the user's host AI. This pack does not prove that the project has been installed, run, or validated.

## Project

- canonical_name: `getzep/graphiti`
- capability: Build Real-Time Knowledge Graphs for AI Agents
- expected_user_outcome: Build Real-Time Knowledge Graphs for AI Agents

## Operating Boundaries

- Do not claim that the project has been installed, run, called through an API, or used on local files unless separate evidence proves it.
- Project facts must come from repo evidence, Claim Graph, or explicit source references.
- When a capability is not verified, mark it as unverified instead of completing it as fact.
- publish_status: `publishable`
- blocking_gaps: none

---

## Doramagic Context Augmentation

The following sections strengthen the repository context for a host AI. Human Manual data is a reading route, and pitfall notes become operating constraints.

## Human Manual Outline

Usage rule: this is only a reading route and salience signal, not factual authority. Concrete claims must still return to repo evidence or Claim Graph.

Host AI hard rules:
- Do not treat page titles, section order, summaries, or importance values as factual project evidence.
- When explaining the Human Manual outline, state that it is only a reading route or salience signal.
- Capability, installation, compatibility, runtime state, and risk claims must cite repo evidence, source paths, or Claim Graph.

- **Introduction to Graphiti and Core Concepts**: importance `high`
  - source_paths: README.md, graphiti_core/__init__.py, graphiti_core/graphiti.py, graphiti_core/nodes.py, graphiti_core/edges.py
- **Graph Database Backends and Driver Architecture**: importance `high`
  - source_paths: graphiti_core/driver/driver.py, graphiti_core/driver/neo4j_driver.py, graphiti_core/driver/falkordb_driver.py, graphiti_core/driver/kuzu_driver.py, graphiti_core/driver/neptune_driver.py
- **LLM Clients, Embedders, and Cross-Encoders**: importance `high`
  - source_paths: graphiti_core/llm_client/client.py, graphiti_core/llm_client/openai_client.py, graphiti_core/llm_client/anthropic_client.py, graphiti_core/llm_client/gemini_client.py, graphiti_core/llm_client/groq_client.py
- **Deployment, MCP Server, REST Service, and Operations**: importance `high`
  - source_paths: mcp_server/README.md, mcp_server/src/graphiti_mcp_server.py, mcp_server/main.py, server/README.md, server/graph_service/main.py

## Repo Inspection Evidence

- repo_clone_verified: true
- repo_inspection_verified: true
- repo_commit: `40eca368a478e6bd8d8638bfabcb5b8da5ce3a64`
- inspected_files: `uv.lock`, `Dockerfile`, `pyproject.toml`, `README.md`, `docker-compose.yml`, `examples/ecommerce/runner.py`, `examples/opentelemetry/pyproject.toml`, `examples/opentelemetry/README.md`, `examples/opentelemetry/otel_stdout_example.py`, `examples/quickstart/dense_vs_normal_ingestion.py`, `examples/quickstart/quickstart_neptune.py`, `examples/quickstart/quickstart_neo4j.py`, `examples/quickstart/README.md`, `examples/quickstart/quickstart_falkordb.py`, `examples/azure-openai/azure_openai_neo4j.py`, `examples/azure-openai/README.md`, `examples/gliner2/README.md`, `examples/gliner2/gliner2_neo4j.py`, `examples/podcast/podcast_runner.py`, `examples/podcast/transcript_parser.py`

Host AI hard rules:
- Without repo_clone_verified=true, do not claim that the source code has been read.
- Without repo_inspection_verified=true, do not write README, docs, or package-file conclusions as facts.
- Without quick_start_verified=true, do not claim that the Quick Start path has run successfully.

## Doramagic Pitfall Constraints

These rules come from Doramagic discovery, validation, or compilation findings. The host AI must treat them as operating constraints, not background notes.

### Constraint 1: Installation risk requires verification

- Trigger: Project evidence flags a installation risk. Review the linked source before relying on this workflow.
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: community_evidence:github | https://github.com/getzep/graphiti/issues/1259
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 2: Security or permission risk requires verification

- Trigger: Project evidence flags a security or permission risk. Review the linked source before relying on this workflow.
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: community_evidence:github | https://github.com/getzep/graphiti/issues/868
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 3: Configuration risk requires verification

- Trigger: Project evidence flags a configuration risk. Review the linked source before relying on this workflow.
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: capability.host_targets | github_repo:840056306 | https://github.com/getzep/graphiti
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 4: Configuration risk requires verification

- Trigger: Project evidence flags a configuration risk. Review the linked source before relying on this workflow.
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: community_evidence:github | https://github.com/getzep/graphiti/issues/1574
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 5: Capability evidence risk requires verification

- Trigger: README/documentation is current enough for a first validation pass.
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: capability.assumptions | github_repo:840056306 | https://github.com/getzep/graphiti
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 6: Maintenance risk requires verification

- Trigger: Project evidence flags a maintenance risk. Review the linked source before relying on this workflow.
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: evidence.maintainer_signals | github_repo:840056306 | https://github.com/getzep/graphiti
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 7: Security or permission risk requires verification

- Trigger: no_demo
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: downstream_validation.risk_items | github_repo:840056306 | https://github.com/getzep/graphiti
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 8: Security or permission risk requires verification

- Trigger: no_demo
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: risks.scoring_risks | github_repo:840056306 | https://github.com/getzep/graphiti
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 9: Maintenance risk requires verification

- Trigger: issue_or_pr_quality=unknown。
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: evidence.maintainer_signals | github_repo:840056306 | https://github.com/getzep/graphiti
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 10: Maintenance risk requires verification

- Trigger: release_recency=unknown。
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: evidence.maintainer_signals | github_repo:840056306 | https://github.com/getzep/graphiti
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

