{
  "info": {
    "name": "Entertainment Express Get Most Active Visitors by IP.",
    "_postman_id": "94e80128-39d7-4018-8cda-5a52aecf4684",
    "description": "No required parameters, DateValue defaults to Today.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analytics",
      "item": [
        {
          "id": "f75f4125-2cb0-48d5-9fa6-5ee37f2f76ec",
          "name": "GetAnalyticsMostActive",
          "request": {
            "url": "http://ee.iva-api.com/Analytics/MostActive/?DateValue=%7B%7D&Limit=%7B%7D&ReportTag=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "No required parameters, DateValue defaults to Today."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "970c49df-9cc4-49ed-9095-02de8e7533d6"
            }
          ]
        }
      ]
    }
  ]
}