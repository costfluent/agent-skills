{
  "id": "crp_Hb7Qe2tLkV0sZ9mYw4RcXg",
  "title": "EC2 by region",
  "chartType": "stackedBar",
  "chartAxis": "date",
  "dateBin": "day",
  "dateInterval": "last30Days",
  "filter": "costs.provider = 'aws' AND costs.service = 'AmazonEC2'",
  "groupBy": [
    {
      "dimension": "Region"
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
  "createdAt": "2026-11-06T09:20:11Z",
  "isDefault": false
}
