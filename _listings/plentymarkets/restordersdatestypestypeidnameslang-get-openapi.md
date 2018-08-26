---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Get a name of an order date type
  description: Gets a name of an order date type. The ID of the date type and the
    language of the name must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/orders/items/{orderItemId}/dates:
    get:
      summary: List dates of an order item
      description: Lists the dates of an order item. The ID of the order item must
        be specified.
      operationId: getRestOrdersItemsOrderitemDates
      x-api-path-slug: restordersitemsorderitemiddates-get
      parameters:
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - List
      - Dates
      - Of
      - Order
      - Item
  /rest/orders/{orderId}/dates:
    get:
      summary: List dates of an order
      description: Lists dates of an order. The ID of the order must be specified.
      operationId: getRestOrdersOrderDates
      x-api-path-slug: restordersorderiddates-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Dates
      - Of
      - Order
  /rest/orders/dates/types:
    get:
      summary: List order date types
      description: List order date types.
      operationId: getRestOrdersDatesTypes
      x-api-path-slug: restordersdatestypes-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Date
      - Types
  /rest/orders/dates/types/{typeId}:
    get:
      summary: Find an order date type by it's ID
      description: Find an order date type by it's id.
      operationId: getRestOrdersDatesTypesType
      x-api-path-slug: restordersdatestypestypeid-get
      parameters:
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Find
      - Order
      - Date
      - Type
      - By
      - Its
      - ID
  /rest/orders/dates/types/{typeId}/names:
    get:
      summary: List names of an order date type
      description: Lists names in all languages available of an order date type. The
        ID of the date type must be specified.
      operationId: getRestOrdersDatesTypesTypeNames
      x-api-path-slug: restordersdatestypestypeidnames-get
      parameters:
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Order
      - Date
      - Type
  /rest/orders/dates/types/{typeId}/names/{lang}:
    get:
      summary: Get a name of an order date type
      description: Gets a name of an order date type. The ID of the date type and
        the language of the name must be specified.
      operationId: getRestOrdersDatesTypesTypeNamesLang
      x-api-path-slug: restordersdatestypestypeidnameslang-get
      parameters:
      - in: path
        name: lang
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Name
      - Of
      - Order
      - Date
      - Type
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---