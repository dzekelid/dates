{
  "info": {
    "name": "Plentymarkets List dates of an order",
    "_postman_id": "6bcd9508-0d07-448b-9bfe-b320e5a2d226",
    "description": "Lists dates of an order. The ID of the order must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "fd472125-00cf-448c-92cc-40ce99e7a051",
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
              "id": "560d043a-17ba-4070-a831-9a7814e548e8"
            }
          ]
        },
        {
          "id": "e654d1a5-926f-4528-b0cc-98aa5f5bf881",
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
              "id": "f88f633a-422b-45cf-bbb1-25586755a4ca"
            }
          ]
        }
      ]
    }
  ]
}