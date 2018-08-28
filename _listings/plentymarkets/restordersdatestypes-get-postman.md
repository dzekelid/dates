{
  "info": {
    "name": "Plentymarkets List order date types",
    "_postman_id": "ac905eea-62ef-4770-8213-c22fcb280ee0",
    "description": "List order date types.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "a83b935d-8106-4d7a-8b7f-a45326f97324",
          "name": "getRestOrdersItemsOrderitemDates",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/items/:orderItemId/dates"
              ],
              "variable": [
                {
                  "id": "orderItemId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Lists the dates of an order item. The ID of the order item must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c95e5cf-2f77-4fa8-b8bc-2e680dd63c95"
            }
          ]
        },
        {
          "id": "e0f251e1-5ec5-4b4a-ad58-7117a3a9e607",
          "name": "getRestOrdersOrderDates",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/:orderId/dates"
              ],
              "variable": [
                {
                  "id": "orderId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Lists dates of an order. The ID of the order must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ef250a5-fcad-4304-96d1-c3ff813bb1c3"
            }
          ]
        },
        {
          "id": "ea04e79b-ce2d-4256-9f61-8cf12d23ddf6",
          "name": "getRestOrdersDatesTypes",
          "request": {
            "url": "http://example.com/rest/orders/dates/types",
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
            "description": "List order date types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01b60041-dffb-40a7-b99b-ca53282a8ca9"
            }
          ]
        }
      ]
    }
  ]
}