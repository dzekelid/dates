swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 1
info:
  title: AWS Device Farm API
  version: 1.0.0
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