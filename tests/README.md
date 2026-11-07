# AWP test plan (draft)

The reference implementation should eventually be assessed with independent checks:

| Category | Check |
| --- | --- |
| Discovery | New client can locate canonical JSON discovery without guessing resource URLs |
| Compatibility | Existing llms.txt consumers still parse the Markdown representation |
| Retrieval | Published structured resources return correct status, content type and valid data |
| Localization | EN/FI/SV equivalents resolve to intended content |
| Redirects | HTTP and HTTPS behavior is logged and verified, including 301/308 chains |
| Faults | Missing and malformed resources yield explicit, testable failures |
| Efficiency | Compare equivalent HTML/JSON transfer sizes and request counts |
| Adoption | Check server logs for actual machine-client usage rather than inferring it |

No benchmark results or compatibility pass claims are recorded here yet.
