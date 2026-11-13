{
  "title": "Terraform",
  "url": "https://docs.costfluent.com/developers/terraform#manage-objects",
  "description": "Manage Costfluent objects as code with its Terraform provider, connect cloud accounts in the same apply, and bring objects made in the product under Terraform.",
  "markdown": "## Manage objects\n\n| Resource | What it manages |\n|---|---|\n| `costfluent_workspace` | A workspace, its currency settings, time zone and automatic syncing |\n| `costfluent_provider` | A connection to a cloud account |\n| `costfluent_workspace_provider` | A connection enabled in a workspace, and which of its accounts the workspace reads |\n| `costfluent_gcp_service_account` | The Google Cloud service account Costfluent runs for your organization |\n| `costfluent_cost_report` | A saved cost report |\n| `costfluent_business_metric` | A business metric a report charts cost per unit of; its values are imported by CSV or the API |\n| `costfluent_folder` | A report folder |\n| `costfluent_dashboard` | A dashboard, and the saved filter its report widgets are read through |\n| `costfluent_dashboard_widget` | A widget on a dashboard: a saved cost report shown as a chart, table or KPI, or text |\n| `costfluent_saved_filter` | A saved filter |\n| `costfluent_savings_view` | A saved view of a workspace's savings queue: a tab and its filters under a title |\n| `costfluent_budget` | A budget and its thresholds |\n| `costfluent_cost_alert` | A cost alert |\n| `costfluent_segment` | A segment |\n| `costfluent_allocation_rule` | An allocation rule |\n| `costfluent_virtual_tag` | A virtual tag |\n| `costfluent_tag_policy` | A workspace's tag policy: the required keys its cost must carry |\n| `costfluent_cost_report_subscription` | A cost report sent to notification channels on a schedule |\n| `costfluent_app` | A notification channel: email, Slack, Microsoft Teams or a webhook |\n| `costfluent_team` | A team |\n| `costfluent_team_member` | A member of the organization in one team, with their role there |\n| `costfluent_team_workspace_access` | A team's access to one workspace, and the dashboard its members open there |\n\nData sources read workspaces, connections, cost data, cost summaries, anomalies, the findings in a workspace's savings queue (`costfluent_savings_items`), your plan's entitlements, and what an AWS role must trust (`costfluent_aws_provider_info`).\n\n<FeatureStatus feature=\"CommitmentCoverage\" />\n\n`costfluent_commitments` reads the reservations, savings plans and committed use discounts a workspace's connections hold.\n\nA workspace with a report and a budget:\n\n```hcl\nresource \"costfluent_workspace\" \"production\" {\n  name     = \"Production\"\n  currency = \"EUR\"\n}\n\nresource \"costfluent_cost_report\" \"by_service\" {\n  workspace_id  = costfluent_workspace.production.id\n  title         = \"Monthly cost by service\"\n  date_interval = \"ThisMonth\"\n  date_bin      = \"Day\"\n  group_by      = [{ dimension = \"ServiceName\" }]\n}\n\nresource \"costfluent_budget\" \"monthly\" {\n  workspace_id = costfluent_workspace.production.id\n  name         = \"Monthly cloud budget\"\n  amount       = 10000\n  currency     = \"EUR\"\n  start_date   = \"2026-01-01\"\n  alerts = [\n    { threshold_percent = 80 },\n    { threshold_percent = 100 },\n  ]\n}\n```\n\n",
  "sections": [
    {
      "heading": "Before you start",
      "url": "https://docs.costfluent.com/developers/terraform#before-you-start"
    },
    {
      "heading": "Create a token",
      "url": "https://docs.costfluent.com/developers/terraform#create-a-token"
    },
    {
      "heading": "Configure the provider",
      "url": "https://docs.costfluent.com/developers/terraform#configure-the-provider"
    },
    {
      "heading": "Connect AWS in the same apply",
      "url": "https://docs.costfluent.com/developers/terraform#connect-aws-in-the-same-apply"
    },
    {
      "heading": "Manage objects",
      "url": "https://docs.costfluent.com/developers/terraform#manage-objects"
    },
    {
      "heading": "Bring existing objects under Terraform",
      "url": "https://docs.costfluent.com/developers/terraform#bring-existing-objects-under-terraform"
    },
    {
      "heading": "How it behaves",
      "url": "https://docs.costfluent.com/developers/terraform#how-it-behaves"
    },
    {
      "heading": "Related",
      "url": "https://docs.costfluent.com/developers/terraform#related"
    }
  ]
}
