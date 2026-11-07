# AWP specification — scope (draft)

## Goal

Define an interoperable, JSON-first way for machine clients to **discover**, **resolve**, and **retrieve** information published by a website without having to reconstruct the information model from rendered HTML.

## In scope

- Canonical machine-readable discovery metadata.
- Explicit mapping between resources and the addresses used to retrieve them.
- Language variants and equivalent human-readable locations.
- A compatibility representation for existing `llms.txt` consumers.
- Documented HTTP-level behavior and validation.
- Optional mapping to external symbol namespaces.

## Out of scope for the initial core

- Requiring AIGMos, Symbolic Memory, a specific CMS or a specific runtime.
- Requiring authentication, MCP or an autonomous bot framework.
- Promising indexing, ranking, traffic savings or crawler adoption.
- Replacing robots.txt or access-control mechanisms.

## Not decided yet

- Canonical JSON discovery filename, location and media type.
- Minimum fields, version negotiation and schema.
- Resource representation and mapping contract.
- Required versus optional language and link metadata.
- Whether and how HTTP `Link` headers advertise the JSON manifest.
- Redirect, caching, and update semantics.

These are explicit design questions, **not implied requirements**.

## Conformance model

Define tests for publication, discovery, retrieval, parsing, cross-language mapping and backward compatibility only after the normative contract is settled.
