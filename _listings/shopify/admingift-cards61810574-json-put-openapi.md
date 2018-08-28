---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Update the expiry date of a gift card
  description: Update the expiry date of a gift card.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/gift_cards/61810574.json:
    put:
      summary: Update the expiry date of a gift card
      description: Update the expiry date of a gift card.
      operationId: putAdminGiftCards61810574.json
      x-api-path-slug: admingift-cards61810574-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Expiry
      - Date
      - Gift
      - Card
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