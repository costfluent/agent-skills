{
  "results": [
    {
      "title": "Terraform",
      "heading": "Manage objects",
      "url": "https://docs.costfluent.com/developers/terraform#manage-objects",
      "excerpt": "| Resource | What it manages | |---|---| | `costfluent_workspace` | A workspace, its currency settings, time zone and automatic syncing | | `costfluent_provider` | A connection to a cloud account | | `costfluent_workspace_provider` | A connection enabled in a workspace, and which of its accounts…"
    },
    {
      "title": "Terraform",
      "heading": "Bring existing objects under Terraform",
      "url": "https://docs.costfluent.com/developers/terraform#bring-existing-objects-under-terraform",
      "excerpt": "An object made in the product, or through the Public API, can be managed by Terraform without recreating it. Write its `resource` block first, then import it by ID with `terraform import` or an `import` block: ```bash terraform import costfluent_cost_report.by_service wsp_1a2b3c:crp_4d5e6f ```…"
    },
    {
      "title": "Budgets",
      "heading": "Before you start",
      "url": "https://docs.costfluent.com/planning/budgets#before-you-start",
      "excerpt": "- Creating, editing and deleting budgets needs the Editor team role in a workspace your team can edit. Every team role can view them. - A budget measures the cost, or the usage, of the connections the workspace uses; see Manage connections."
    }
  ]
}
