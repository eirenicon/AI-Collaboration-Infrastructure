# Memory Schema Specification (Draft)

This document defines the structure, semantics, and handling protocols for memory entries used in collaborative AI systems.

## Goals

- Semantic clarity
- Git-friendly diffs
- Cross-agent compatibility
- Human readability
- Degradation resilience

## Top-Level Structure

Each memory entry is a JSON object with the following fields:

```json
{
  "id": "uuid-v4",
  "agent": "agent-name-or-id",
  "timestamp": "ISO-8601",
  "content": "string or object",
  "tags": ["string"],
  "hash": "sha256",
  "version": "v0.1.0"
}
