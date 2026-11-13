{
  "currency": "USD",
  "level": "workload",
  "rows": [
    {
      "cluster": "prod-eu-1",
      "namespace": "__idle__",
      "workload": "",
      "cost": "1840.20000000",
      "idleCost": "1840.20000000",
      "cpu": {
        "requested": 0,
        "used": 0,
        "peak": 0
      },
      "memory": {
        "requested": 0,
        "used": 0,
        "peak": 0
      }
    },
    {
      "cluster": "prod-eu-1",
      "namespace": "search",
      "workload": "Deployment/search-indexer",
      "cost": "1210.55000000",
      "idleCost": "0E-8",
      "cpu": {
        "requested": 5760,
        "used": 1094.4,
        "peak": 1958.4,
        "usedPercent": 19.0,
        "peakPercent": 34.0
      },
      "memory": {
        "requested": 23040,
        "used": 9216,
        "peak": 12441.6,
        "usedPercent": 40.0,
        "peakPercent": 54.0
      }
    },
    {
      "cluster": "prod-eu-1",
      "namespace": "checkout",
      "workload": "Deployment/checkout-api",
      "cost": "980.30000000",
      "idleCost": "0E-8",
      "cpu": {
        "requested": 2880,
        "used": 2534.4,
        "peak": 3772.8,
        "usedPercent": 88.0,
        "peakPercent": 131.0
      },
      "memory": {
        "requested": 11520,
        "used": 8870.4,
        "peak": 10483.2,
        "usedPercent": 77.0,
        "peakPercent": 91.0
      }
    },
    {
      "cluster": "prod-eu-1",
      "namespace": "data",
      "workload": "StatefulSet/kafka",
      "cost": "860.10000000",
      "idleCost": "0E-8",
      "cpu": {
        "requested": 2160,
        "used": 1036.8,
        "peak": 1490.4,
        "usedPercent": 48.0,
        "peakPercent": 69.0
      },
      "memory": {
        "requested": 17280,
        "used": 12441.6,
        "peak": 14169.6,
        "usedPercent": 72.0,
        "peakPercent": 82.0
      }
    },
    {
      "cluster": "prod-eu-1",
      "namespace": "monitoring",
      "workload": "StatefulSet/prometheus",
      "cost": "312.45000000",
      "idleCost": "0E-8",
      "cpu": {
        "requested": 720,
        "used": 489.6,
        "peak": 655.2,
        "usedPercent": 68.0,
        "peakPercent": 91.0
      },
      "memory": {
        "requested": 5760,
        "used": 4953.6,
        "peak": 5587.2,
        "usedPercent": 86.0,
        "peakPercent": 97.0
      }
    },
    {
      "cluster": "prod-eu-1",
      "namespace": "batch",
      "workload": "Pod/reindex-20261103",
      "cost": "92.10000000",
      "idleCost": "0E-8",
      "cpu": {
        "requested": 96,
        "used": 88.3,
        "peak": 96,
        "usedPercent": 91.98,
        "peakPercent": 100.0
      },
      "memory": {
        "requested": 384,
        "used": 207.4,
        "peak": 268.8,
        "usedPercent": 54.01,
        "peakPercent": 70.0
      }
    }
  ],
  "truncated": false,
  "unconverted": []
}
