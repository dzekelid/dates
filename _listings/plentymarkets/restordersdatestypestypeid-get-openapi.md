---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Find an order date type by it's ID
  description: Find an order date type by it's id.
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
  /rest/orders/items/dates/{id}:
    delete:
      summary: Delete a date from an order item
      description: Deletes the date from an order item. The ID of the date must be
        specified.
      operationId: deleteRestOrdersItemsDates
      x-api-path-slug: restordersitemsdatesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Date
      - From
      - Order
      - Item
    get:
      summary: Get a date of an order item
      description: Gets a date of an order item. The ID of the date must be specified.
      operationId: getRestOrdersItemsDates
      x-api-path-slug: restordersitemsdatesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
    put:
      summary: Update a date of an order item
      description: Updates a date of an order item. The ID of the date must be specified.
      operationId: putRestOrdersItemsDates
      x-api-path-slug: restordersitemsdatesid-put
      parameters:
      - in: body
        name: /rest/orders/items/dates/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
  /rest/orders/items/{orderItemId}/dates/{typeId}:
    delete:
      summary: Delete a date from an order item by order item and date type
      description: Deletest a date from an order item. The ID of the order item and
        the ID of the date type must be specified.
      operationId: deleteRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-delete
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Date
      - From
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
    get:
      summary: Get a date of an order item by order item and date type
      description: Gets a date of an order item. The ID of the order item and the
        ID of the date type must be specified.
      operationId: getRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-get
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
    post:
      summary: Create a date for an order item by order item and date type
      description: Creates a date for an order item. The ID of the order item and
        the ID of the date type must be specified.
      operationId: postRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-post
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/dates/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Datean
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
    put:
      summary: Update a date of an order item by order item and date type
      description: Updates the date of an order item. The ID of the order item and
        the ID of the date type must be specified.
      operationId: putRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-put
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/dates/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
  /rest/orders/{orderId}/dates/{typeId}:
    get:
      summary: Get a date
      description: Gets a date. The ID of the order and the ID of the date type must
        be specified.
      operationId: getRestOrdersOrderDatesType
      x-api-path-slug: restordersorderiddatestypeid-get
      parameters:
      - in: path
        name: orderId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Date
  /rest/payments/entrydate:
    get:
      summary: List payments by entry date
      description: Lists all payments by entry date within a certain date range. The
        start and the end of the date range must be specified.
      operationId: getRestPaymentsEntrydate
      x-api-path-slug: restpaymentsentrydate-get
      parameters:
      - in: query
        name: endDate
        description: The end date of the date range for the entry date of the payment
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: startDate
        description: The start date of the date range for the entry date of the payment
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - By
      - Entry
      - Date
  /rest/payments/importdate:
    get:
      summary: List payments by import date
      description: Lists all payments by import date within a certain date range.
        The start and the end of the date range must be specified.
      operationId: getRestPaymentsImportdate
      x-api-path-slug: restpaymentsimportdate-get
      parameters:
      - in: query
        name: endDate
        description: The end date of the date range for the import date of the payment
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: startDate
        description: The start date of the date range for the import date of the payment
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - By
      - Import
      - Date
  /rest/payments/properties/date:
    get:
      summary: List properties by creation date
      description: Lists all properties by creation date. The start and the end of
        the date range must be specified.
      operationId: getRestPaymentsPropertiesDate
      x-api-path-slug: restpaymentspropertiesdate-get
      parameters:
      - in: query
        name: endDate
        description: The end date of the date range for the date of creation of the
          property
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: startDate
        description: The start date of the date range for the date of creation of
          the property
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
      - By
      - Creation
      - Date
  /rest/orders/items/dates:
    post:
      summary: Create a date for an order item
      description: Creates a date for an order item. The ID of the order item must
        be specified
      operationId: postRestOrdersItemsDates
      x-api-path-slug: restordersitemsdates-post
      parameters:
      - in: body
        name: /rest/orders/items/dates
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datean
      - Order
      - Item
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