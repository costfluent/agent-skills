{
  "items": [
    {
      "id": "ano_QMU5ekzu9WhvimCT_hzXHg",
      "workspaceId": "wsp_XG-lR2vXB7Ma_bvUomUv2w",
      "providerId": "prv_HxgfmT5y-D5XNfAFZJOGzQ",
      "anomalyDate": "2026-11-02",
      "serviceName": "Amazon Elastic Compute Cloud",
      "region": "us-east-1",
      "anomalyType": "spike",
      "severity": "high",
      "expectedCost": "412.37000000",
      "actualCost": "978.61000000",
      "deviationPercent": 137.31,
      "description": "Amazon Elastic Compute Cloud cost in us-east-1 rose well above its 30-day baseline.",
      "currency": "USD",
      "status": "open",
      "isAcknowledged": false,
      "detectedAt": "2026-11-05T04:00:11Z",
      "contributors": [
        {
          "accountId": "210987654321",
          "resourceId": "i-0c7f3a91d2e4b5a60",
          "increase": "188.40000000"
        },
        {
          "accountId": "210987654321",
          "resourceId": "i-0c7f3a91d2e4b5a61",
          "increase": "176.95000000"
        },
        {
          "accountId": "210987654321",
          "resourceId": "i-0c7f3a91d2e4b5a62",
          "increase": "171.10000000"
        }
      ],
      "attributedSku": "USE1-BoxUsage:c7i.4xlarge",
      "skuContributors": [
        {
          "sku": "USE1-BoxUsage:c7i.4xlarge",
          "increase": "498.20000000"
        },
        {
          "sku": "USE1-EBS:VolumeUsage.gp3",
          "increase": "41.30000000"
        },
        {
          "sku": "USE1-DataTransfer-Regional-Bytes",
          "increase": "18.75000000"
        }
      ]
    },
    {
      "id": "ano_rSOyZm86onYq3OykAnEZlA",
      "workspaceId": "wsp_XG-lR2vXB7Ma_bvUomUv2w",
      "providerId": "prv_I3OYAm91u2bgiam4UqEEug",
      "anomalyDate": "2026-10-21",
      "serviceName": "Virtual Machines",
      "region": "uaenorth",
      "anomalyType": "spike",
      "severity": "low",
      "expectedCost": "1081.40000000",
      "actualCost": "1395.50000000",
      "deviationPercent": 29.05,
      "description": "Virtual Machines cost in uaenorth rose above its 30-day baseline.",
      "currency": "AED",
      "status": "acknowledged",
      "isAcknowledged": true,
      "acknowledgedAt": "2026-10-24T09:41:00Z",
      "detectedAt": "2026-10-24T04:00:09Z",
      "contributors": [
        {
          "accountId": "5f2a7c1e-3b9d-4e8a-a6c0-1d2e3f4a5b6c",
          "resourceId": "/subscriptions/5f2a7c1e-3b9d-4e8a-a6c0-1d2e3f4a5b6c/resourceGroups/rg-batch/providers/Microsoft.Compute/virtualMachines/vm-batch-07",
          "increase": "244.10000000"
        }
      ],
      "attributedResourceId": "/subscriptions/5f2a7c1e-3b9d-4e8a-a6c0-1d2e3f4a5b6c/resourceGroups/rg-batch/providers/Microsoft.Compute/virtualMachines/vm-batch-07",
      "skuContributors": [
        {
          "sku": "D8s v5",
          "increase": "251.30000000"
        }
      ]
    }
  ]
}
