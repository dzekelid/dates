{
  "info": {
    "name": "Google Safe Browsing API Encoded Updates",
    "_postman_id": "e8fc18dc-6cf1-4e52-9d09-e17b4e88dfb0",
    "description": "Encoded Updates",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "updates",
      "item": [
        {
          "id": "7addb868-6686-4429-8f5f-4f9930bf761d",
          "name": "safebrowsing.encodedUpdates.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "safebrowsing.googleapis.com",
              "path": [
                "v4/encodedUpdates/:encodedRequest"
              ],
              "query": [
                {
                  "key": "clientId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "clientVersion",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "encodedRequest",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Encoded Updates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fae5c70-ff0e-4169-ba54-12b8b224b37a"
            }
          ]
        }
      ]
    }
  ]
}