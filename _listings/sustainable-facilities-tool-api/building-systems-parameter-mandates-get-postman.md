{
  "info": {
    "name": "Sustainable Facilities Tool API Building System Mandate",
    "_postman_id": "35482cbd-c148-4799-8cfa-2487c360bff8",
    "description": "Returns a building system mandate by parameter.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "mandates",
      "item": [
        {
          "id": "814b2a34-3105-4c71-921e-aec4293dc4c5",
          "name": "returnBuildingSystemMandate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.gov",
              "path": [
                "sftool",
                "v1",
                "building-systems/:parameter/mandates"
              ],
              "variable": [
                {
                  "id": "parameter",
                  "value": "parameter",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a building system mandate by parameter"
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
              "body": "[\r\n  {\r\n    \"id\": 246,\r\n    \"name\": \"name\"\r\n  }\r\n]",
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "2d0c8171-8657-49b3-9ece-b2295857b18d"
            }
          ]
        }
      ]
    }
  ]
}