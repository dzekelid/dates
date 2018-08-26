---
swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 0
info:
  title: AWS Device Farm API Renew Offering
  version: 1.0.0
  description: |-
    Explicitly sets the quantity of devices to renew for an offering, starting from the
          effectiveDate of the next period.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RenewOffering:
    get:
      summary: Renew Offering
      description: |-
        Explicitly sets the quantity of devices to renew for an offering, starting from the
              effectiveDate of the next period.
      operationId: renewOffering
      x-api-path-slug: actionrenewoffering-get
      parameters:
      - in: query
        name: offeringId
        description: The ID of a request to renew an offering
        type: string
      - in: query
        name: quantity
        description: The quantity requested in an offering renewal
        type: string
      responses:
        200:
          description: OK
      tags:
      - Offerings
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