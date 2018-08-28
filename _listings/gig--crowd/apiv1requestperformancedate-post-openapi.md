---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Post Request Performancedate
  version: 1.0.0
  description: Post request performancedate.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/request/art/accept/performanceDate:
    post:
      summary: Post Request Art Accept Performancedate
      description: Post request art accept performancedate.
      operationId: postApiV1RequestArtAcceptPerformancedate
      x-api-path-slug: apiv1requestartacceptperformancedate-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        description: /
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Request
      - Art
      - Accept
      - Performancedate
  /api/v1/request/art/reject/performanceDate:
    post:
      summary: Post Request Art Reject Performancedate
      description: Post request art reject performancedate.
      operationId: postApiV1RequestArtRejectPerformancedate
      x-api-path-slug: apiv1requestartrejectperformancedate-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        description: /
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Request
      - Art
      - Reject
      - Performancedate
  /api/v1/request/performanceDate:
    post:
      summary: Post Request Performancedate
      description: Post request performancedate.
      operationId: postApiV1RequestPerformancedate
      x-api-path-slug: apiv1requestperformancedate-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Request
      - Performancedate
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