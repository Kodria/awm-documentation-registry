# Context Kernel v1 Migration

Date: 2026-09-22

The repository owner explicitly approved migration to the current AWM context contract. The AWM-managed block is generated runtime context, remains visible outside the protected region, and is excluded from the owner-authored legacy inventory.

## Block Inventory

| Legacy block ID | Source range / hash | Context ID | Destination | Rationale |
| --- | --- | --- | --- | --- |
| LEGACY-AGENTS-001 | `AGENTS.md:1-1` / `sha256:204aa1e75dc7abd78c37fb0bbf9d946d41ff6f0ce819c299be2b5f903665f8d3` | `CTX-AGENTS-001` | `AGENTS.md` protected kernel | Retained verbatim as unconditional repository context. |
| LEGACY-AGENTS-002 | `AGENTS.md:3-3` / `sha256:abc500c11f1910d239c818c05aac9fcfd93797194627d6b01baa6e8137d29bf8` | `CTX-AGENTS-002` | `AGENTS.md` protected kernel | Retained verbatim as unconditional repository context. |
| LEGACY-AGENTS-003 | `AGENTS.md:5-5` / `sha256:f3f9e1151c83d22bbdfc4b0af15ee26e0285596817d4b061dcc098484f60960c` | `CTX-AGENTS-003` | `AGENTS.md` protected kernel | Retained verbatim as unconditional repository context. |
| LEGACY-AGENTS-004 | `AGENTS.md:7-7` / `sha256:1aa27a8ac4e6b16d8607761f7ddc936d0ef6116c49bba1405ec8a7d905804af2` | `CTX-AGENTS-004` | `AGENTS.md` protected kernel | Retained verbatim as unconditional repository context. |
| LEGACY-AGENTS-005 | `AGENTS.md:9-11` / `sha256:b9c0d3c7a3eccf064eea73bd5a9125fb310cfe27bf5b3b7a45d6d3b847686dbc` | `CTX-AGENTS-005` | `AGENTS.md` protected kernel | Retained verbatim as unconditional repository context. |
| LEGACY-AGENTS-006 | `AGENTS.md:13-13` / `sha256:ae08eb6786300787c87e5f033e0b1f730bd42bf49e956558fc8f187eadea1cfa` | `CTX-AGENTS-006` | `AGENTS.md` protected kernel | Retained verbatim as unconditional repository context. |
| LEGACY-AGENTS-007 | `AGENTS.md:15-19` / `sha256:7ded54b7f454ad3e366c98ba83d38b86939ddab1a36da4b30e02ee471a626c26` | `CTX-AGENTS-007` | `AGENTS.md` protected kernel | Retained verbatim as unconditional repository context. |
| LEGACY-AGENTS-008 | `AGENTS.md:21-21` / `sha256:528c2ac07d3e224d8c88c51411112f68665d2dbb0c4f356ab0ec8a1ae81e138d` | `CTX-AGENTS-008` | `AGENTS.md` protected kernel | Retained verbatim as unconditional repository context. |
| LEGACY-AGENTS-009 | `AGENTS.md:23-26` / `sha256:4e58d5f65d5809a37f28b2004a81fa9be77f0afeeb51937da1a6e46594083b8a` | `CTX-AGENTS-009` | `AGENTS.md` protected kernel | Retained verbatim as unconditional repository context. |
| LEGACY-AGENTS-010 | `AGENTS.md:28-28` / `sha256:1f6be1ef8d8afe0b7eab56da42511169c1f86b90035f7e8fd611e168aaeb0c58` | `CTX-AGENTS-010` | `AGENTS.md` protected kernel | Retained verbatim as unconditional repository context. |
| LEGACY-AGENTS-011 | `AGENTS.md:30-32` / `sha256:ab6949210c1336c555b13c4d14273ab2f537b40cab5ac892a22da33d8f3afa1d` | `CTX-AGENTS-011` | `AGENTS.md` protected kernel | Retained verbatim as unconditional repository context. |

## Inventory Equality

- Pre-migration Context IDs: `CTX-AGENTS-001`, `CTX-AGENTS-002`, `CTX-AGENTS-003`, `CTX-AGENTS-004`, `CTX-AGENTS-005`, `CTX-AGENTS-006`, `CTX-AGENTS-007`, `CTX-AGENTS-008`, `CTX-AGENTS-009`, `CTX-AGENTS-010`, `CTX-AGENTS-011`.
- Post-migration Context IDs: `CTX-AGENTS-001`, `CTX-AGENTS-002`, `CTX-AGENTS-003`, `CTX-AGENTS-004`, `CTX-AGENTS-005`, `CTX-AGENTS-006`, `CTX-AGENTS-007`, `CTX-AGENTS-008`, `CTX-AGENTS-009`, `CTX-AGENTS-010`, `CTX-AGENTS-011`.
- Result: equal; no owner-authored block was removed or split across IDs.
