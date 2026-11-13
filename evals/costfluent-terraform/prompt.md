---
description: Write HCL that connects a Google Cloud billing export, without applying it, and check which providers land cost
max_turns: 15
allowed_tools: [Skill]
---

Show me the Terraform to connect our Google Cloud billing export to Costfluent next to the AWS
connection we already have. The export is in project acme-billing, dataset billing_export, billing
account 012345-ABCDEF-678901. Don't run anything against our accounts. Then tell me which providers
already land cost in the Production workspace this month.
