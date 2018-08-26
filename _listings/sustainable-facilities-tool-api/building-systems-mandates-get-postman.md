{
  "info": {
    "name": "Sustainable Facilities Tool API Building System Mandates",
    "_postman_id": "a4691643-ad02-4a39-ac8e-b8579dd489d0",
    "description": "Returns all building systems mandates",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "mandates",
      "item": [
        {
          "id": "c0cfc2f7-dda2-4f23-b2c7-62a5a3936891",
          "name": "returnBuildingSystemMandates",
          "request": {
            "url": "http://api.data.gov/sftool/v1/building-systems/mandates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all building systems mandates"
          },
          "response": [
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "[\r\n  {\r\n    \"id\": 225,\r\n    \"name\": \"name\"\r\n  }\r\n]",
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "94e44824-f11f-46ca-ad0e-fa1c880938c5"
            }
          ]
        }
      ]
    }
  ]
}