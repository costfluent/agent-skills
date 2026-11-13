---
type: llm
weight: 1
---

The response passes when all of these hold:

- The HCL uses the costfluent/costfluent provider pinned to a version, a costfluent_gcp_service_account
  resource, the costfluent/cost-access/gcp module with the project, dataset, billing account and the
  service account's email, and a costfluent_provider with key "gcp" fed by the module's credentials
  (and settings), depending on the module.
- No token or secret is written literally: the token comes from the COSTFLUENT_API_KEY environment
  variable or a sensitive variable.
- It does not run or claim to have run terraform apply, and leaves applying to the person.
- It says the new connection's cost shows only in the workspaces it is associated with, and that
  the first cost takes time to arrive.
- From the tool results it reports AWS cost landing this month and Azure cost billed in AED that is
  left out of the USD total rather than zero, and says Google Cloud has no cost there yet because it
  is not connected, without calling that zero spend.
- It does not invent figures that no tool returned.
