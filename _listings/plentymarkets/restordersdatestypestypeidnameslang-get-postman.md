{
  "info": {
    "name": "Plentymarkets Get a name of an order date type",
    "_postman_id": "4f290645-4730-4779-a9a1-fe4843e6c539",
    "description": "Gets a name of an order date type. The ID of the date type and the language of the name must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "eec61b4e-af72-4c70-8084-1655c3dbb842",
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
              "id": "5001ff78-add8-4820-a6e7-e0440805fe32"
            }
          ]
        },
        {
          "id": "35c565e4-efad-411e-8082-1a370aab90d1",
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
              "id": "b4be906c-cefe-49e2-904f-70bd89b99a98"
            }
          ]
        },
        {
          "id": "076dfb53-d19f-4b03-bb19-a5901f18d673",
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
              "id": "c65042a5-8f9b-4528-897a-adede23b9219"
            }
          ]
        },
        {
          "id": "fe2414b7-594a-4291-a733-e5e4679b7179",
          "name": "getRestOrdersDatesTypesTypeNames",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/dates/types/:typeId/names"
              ],
              "variable": [
                {
                  "id": "typeId",
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
            "description": "Lists names in all languages available of an order date type. The ID of the date type must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2bfe704a-3622-4efc-927c-a3c945fe7efb"
            }
          ]
        }
      ]
    },
    {
      "name": "Find",
      "item": [
        {
          "id": "566c3d46-d692-497f-b12c-9ea72d5e8d58",
          "name": "getRestOrdersDatesTypesType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/dates/types/:typeId"
              ],
              "variable": [
                {
                  "id": "typeId",
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
            "description": "Find an order date type by it's id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6153341-818b-46d9-8321-630bb071e76e"
            }
          ]
        }
      ]
    },
    {
      "name": "Name",
      "item": [
        {
          "id": "d6751b77-86ac-4552-9255-d3c6ab0abe1f",
          "name": "getRestOrdersDatesTypesTypeNamesLang",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/dates/types/:typeId/names/:lang"
              ],
              "variable": [
                {
                  "id": "lang",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "typeId",
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
            "description": "Gets a name of an order date type. The ID of the date type and the language of the name must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea739bd6-20cb-46b8-b548-6ece3e7d8708"
            }
          ]
        }
      ]
    }
  ]
}