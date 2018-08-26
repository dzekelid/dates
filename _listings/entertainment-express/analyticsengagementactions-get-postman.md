{
  "info": {
    "name": "Entertainment Express GetAnalyticEngagementActions",
    "_postman_id": "94dc80f3-716d-4210-a316-3309d17649c3",
    "description": "No required parameters, DateValue defaults to Today.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analytics",
      "item": [
        {
          "id": "6731b829-0190-4c8c-9029-36c3a690cd43",
          "name": "GetAnalyticEngagementActions",
          "request": {
            "url": "http://ee.iva-api.com/Analytics/EngagementActions/?DateValue=%7B%7D&End=%7B%7D&Limit=%7B%7D&ReportTag=%7B%7D&Start=%7B%7D",
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
              "id": "2a4bd2d7-67ce-4b13-a4f0-e40324c932b5"
            }
          ]
        }
      ]
    }
  ]
}