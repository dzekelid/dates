---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
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
---