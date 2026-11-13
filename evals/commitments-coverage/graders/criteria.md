---
type: llm
weight: 1
---

The response passes when all of these hold:

- It says the figures start at 2026-05-01, where the plan's history begins, so they cover about six
  months, not twelve, and it does not fill the earlier months with zero.
- It says the figures leave out about 203,419 AED of spend with no exchange rate, so the Azure usage
  is missing from coverage rather than uncovered.
- It reports AWS coverage falling from 72.4% in May to 61.7% in October, with the effective savings
  rate and utilization from the result.
- It flags the Compute Savings Plan that ends on 2026-11-28 (19 days) and says coverage will drop
  further unless it is replaced, and the RDS reservation at 61.2% utilization with about 254 USD
  unused over 30 days.
- It presents any purchase recommendation as an estimate from its source, keeps the Azure
  reservation finding's 1,650 AED apart from USD figures, and does not claim a purchase is certain to
  pay off.
- It does not invent figures that no tool returned.
