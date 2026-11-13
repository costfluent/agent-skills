---
type: llm
weight: 1
---

The response passes when all of these hold:

- It recommends open findings in a reasoned order, citing estimated monthly saving with confidence,
  risk and effort, for example the m5.4xlarge rightsizing (412.80 USD a month, high confidence, low
  risk) ahead of riskier work.
- It reports the verified saving as 214.75 USD a month from the S3 Intelligent-Tiering finding
  alone, and does not count any estimate as saved.
- It says the implemented gp2 volume deletion (estimate 327.68 USD) has no measurement yet, so its
  saving is not known, and does not report it as saved or as zero saved.
- It keeps the Azure reservation's estimate in AED (1,650 AED) apart and never adds it to USD
  amounts.
- It does not claim it can accept, implement or decline a finding itself; changing a finding's
  state is left to a person in the app.
- It does not invent figures that no tool returned.
