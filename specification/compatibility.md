# Compatibility with llms.txt

AWP is a proposed extension to the machine-readable web ecosystem, **not a claim that the existing llms.txt specification is invalid**.

The [Answer.AI llms.txt v2 proposal](https://github.com/AnswerDotAI/llms-txt) uses Markdown with a structured H1/H2/link-list convention. It recommends `rel="describedby"` for the applicable llms.txt and `rel="alternate"` for Markdown page variants.

## Proposed direction

- JSON is AWP's **canonical discovery representation**.
- Markdown `llms.txt` is a **generated or otherwise synchronized compatibility view**.
- Existing llms.txt clients can keep using the Markdown version.
- New AWP-aware clients should not need Markdown interpretation to understand the structured discovery model.

## What is not settled

This document does **not** yet select a JSON filename, replace the Markdown content at `/llms.txt`, or specify a mandatory negotiation protocol.

A stable JSON schema and backward-compatible publication strategy must be validated before making normative compatibility claims.
