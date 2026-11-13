---
type: llm
weight: 1
---

The response passes when all of these hold:

- It names Deployment/search-indexer as the clearest over-requested workload: 19% of requested CPU
  used and a 34% peak, 40% of requested memory and a 54% peak, at about 1,210.55 USD.
- It reports the idle cost of about 1,840.20 USD as node capacity no container was allocated,
  belonging to the cluster, not to any workload, and says lowering requests alone does not lower
  the bill unless nodes are removed or made smaller.
- It does not recommend cutting Deployment/checkout-api's CPU request: its CPU peak is above 100% of
  the request.
- When it mentions the search-indexer rightsizing finding, it gives its 186.40 USD a month as an
  estimate (accepted, not yet verified), and keeps any saving it works out itself apart from it.
- It does not claim GPU efficiency figures, and does not invent figures that no tool returned.
