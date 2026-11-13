{
  "reports": [
    {
      "id": "crp_sxVx3sov_ecffc_x5Do7_w",
      "title": "AWS by service",
      "chartType": "stackedBar",
      "chartAxis": "date",
      "dateBin": "day",
      "dateInterval": "thisMonth",
      "filter": "costs.provider = 'aws'",
      "groupBy": [
        {
          "dimension": "ServiceName"
        }
      ],
      "settings": {
        "amortize": true,
        "includeCredits": false,
        "includeRefunds": false,
        "includeTax": true,
        "showForecast": false,
        "compareToLastPeriod": true,
        "measure": "cost"
      },
      "createdAt": "2026-03-11T10:02:41Z",
      "updatedAt": "2026-09-30T08:15:12Z",
      "isDefault": false
    },
    {
      "id": "crp_lM9oaFQf6zEyesElA3l2Bg",
      "title": "Kubernetes by namespace",
      "chartType": "bar",
      "chartAxis": "date",
      "dateBin": "week",
      "dateInterval": "last30Days",
      "filter": "costs.provider = 'kubernetes'",
      "groupBy": [
        {
          "dimension": "Cluster"
        },
        {
          "dimension": "Namespace"
        }
      ],
      "settings": {
        "amortize": true,
        "includeCredits": false,
        "includeRefunds": false,
        "includeTax": true,
        "showForecast": false,
        "compareToLastPeriod": true,
        "measure": "cost"
      },
      "createdAt": "2026-04-22T13:47:09Z",
      "isDefault": false
    },
    {
      "id": "crp_n9XSTv-KDksqE4TBPRSO1Q",
      "title": "Cloud spend by provider",
      "chartType": "line",
      "chartAxis": "date",
      "dateBin": "month",
      "dateInterval": "last6Months",
      "groupBy": [
        {
          "dimension": "Provider"
        }
      ],
      "settings": {
        "amortize": true,
        "includeCredits": false,
        "includeRefunds": false,
        "includeTax": true,
        "showForecast": false,
        "compareToLastPeriod": true,
        "measure": "cost"
      },
      "createdAt": "2026-02-03T09:14:22Z",
      "isDefault": true
    }
  ]
}
