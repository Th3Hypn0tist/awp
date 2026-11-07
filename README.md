# AWP — AIGM Agentic Web Pattern

**Status:** Proposal / work in progress · **Version:** 0.1.0-draft

AWP is a proposed **JSON-first** approach to machine-readable web discovery and access. Its purpose is to make public information directly discoverable and addressable by machine clients while keeping conventional human-readable pages available.

## Core principles

1. **JSON is primary.** Structured discovery and resource metadata have one canonical machine-readable representation.
2. **Existing `llms.txt` remains compatible.** Markdown is a secondary compatibility view; it must not become a second source of truth.
3. **Explicit resource mapping.** A client can identify available resources, supported languages, resource addresses, and human equivalents without scraping page layouts.
4. **Implementation-neutral.** Static files and server-generated endpoints must be equally possible.
5. **Optional integration.** AWP does not depend on AIGMos. AIGMos and symbolic-memory mappings are separate examples, not protocol prerequisites.
6. **Measurable behavior.** Discovery, fetch success, response sizes, redirects, and adoption must be tested separately. Reduced traffic is a hypothesis to measure, not a guaranteed outcome.

## What this repository contains

- [Scope and initial requirements](specification/README.md)
- [Discovery proposal](specification/discovery.md)
- [Compatibility with llms.txt](specification/compatibility.md)
- [Validation plan](tests/README.md)

The JSON schema, endpoint names, resource metadata and normative behavior are **not finalized**. They will be defined after the architecture review and proven with a reference implementation.

## Relationship to llms.txt

AWP proposes a JSON-first discovery model that **complements**, rather than replaces, the existing [Answer.AI llms.txt proposal](https://github.com/AnswerDotAI/llms-txt). The existing Markdown conventions should remain consumable by tools that already implement them.

## Reference site

The emerging demonstration is published under [aigm.fi/awp](https://aigm.fi/awp/). A demonstration is not by itself a conformance claim.

## Project layout

```text
AWP/
├── README.md
├── specification/
│   ├── README.md
│   ├── discovery.md
│   └── compatibility.md
└── tests/
    └── README.md
```

AIGM · Architecture before implementation.
