<!-- AWM:CONTEXT-KERNEL:START v1 -->
<!-- awm-context:CTX-AGENTS-001 -->
# AGENTS.md

<!-- awm-context:CTX-AGENTS-002 -->
## Repository Overview

<!-- awm-context:CTX-AGENTS-003 -->
This repository is the AWM documentation content registry. It publishes the `docs` bundle, its orchestrator declaration, reusable documentation skills, agent prompts, and workflow definitions; it does not contain an executable application.

<!-- awm-context:CTX-AGENTS-004 -->
## Validation Commands

<!-- awm-context:CTX-AGENTS-005 -->
- `awm preflight --require-current`: validate the local AWM environment and registry compatibility.
- `awm sensors run --all`: report the repository's explicit content-only sensor opt-out.
- Validate JSON files after editing `awm-registry.json`, `catalog.json`, or `bundles/docs/bundle.json`.

<!-- awm-context:CTX-AGENTS-006 -->
## Directory Structure

<!-- awm-context:CTX-AGENTS-007 -->
- `skills/`: documentation skills and their supporting resources.
- `agents/`: provider-neutral agent prompts.
- `workflows/`: durable workflow definitions.
- `bundles/docs/`: bundle metadata consumed by AWM.
- `awm-registry.json` and `catalog.json`: registry and publication metadata.

<!-- awm-context:CTX-AGENTS-008 -->
## Content Conventions

<!-- awm-context:CTX-AGENTS-009 -->
- Keep instructions provider-neutral and use native runtime capabilities instead of vendor-specific tool names.
- Preserve agreement between the catalog, bundle metadata, orchestrator declaration, and referenced skill names.
- Treat skill instructions and workflow contracts as public interfaces: validate inputs explicitly and fail loudly when required content is missing or malformed.
- Update the relevant bundle metadata whenever published content changes.

<!-- awm-context:CTX-AGENTS-010 -->
## Important Constraints

<!-- awm-context:CTX-AGENTS-011 -->
- Do not add application dependencies or product runtime code to this content-only registry.
- Do not claim local sensor success as release proof; publication validation must be established by the registry's release process.
- Preserve user-authored skill guidance unless the requested change explicitly supersedes it.
<!-- AWM:CONTEXT-KERNEL:END v1 -->
