# Discovery model — design notes

**Status: exploratory; not normative.**

AWP distinguishes four operations:

1. **Discover:** Find the canonical machine-readable resource directory.
2. **Resolve:** Select the exact resource and language needed.
3. **Retrieve:** Fetch the structured response at its declared address.
4. **Interpret:** Consume the returned content according to its defined contract.

The current reference website publishes a root `/llms.txt` that points to JSON resources under `/awp/data/{language}/`. This is a demonstration of direct access, **not yet a finalized AWP discovery protocol**.

## Open design questions

- How does a client discover the JSON-first manifest without first relying on HTML?
- How can an existing `llms.txt` client continue to work unchanged?
- How do redirects (HTTP → HTTPS), content types, errors and caches affect a discovery chain?
- How are equivalent resources associated across languages?
- How can stable resource identifiers be mapped to external symbol systems without making those systems mandatory?

## Engineering constraint

A client must not be required to parse an HTML navigation tree to retrieve a known structured resource. Whether clients actually switch to those resources is an adoption question and must be measured.
