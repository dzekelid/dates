---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 1
info:
  title: LH Public
  version: "1.0"
host: api.lufthansa.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /offers/seatmaps/{flightNumber}/{origin}/{destination}/{date}/{cabinClass}:
    get:
      summary: Seat Maps
      description: Cabin layout and seat characteristics.
      operationId: OffersSeatmapsDestinationDateCabinClassByFlightNumberAndOriginGet
      x-api-path-slug: offersseatmapsflightnumberorigindestinationdatecabinclass-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: cabinClass
        description: 'Cabin class: M, E, C, F'
      - in: path
        name: date
        description: Departure date (YYYY-MM-DD)
      - in: path
        name: destination
        description: Destination airport
      - in: path
        name: flightNumber
        description: Flight number including carrier code and any suffix (e
      - in: path
        name: origin
        description: Departure airport
      responses:
        200:
          description: OK
      tags:
      - Offers
      - Seatmaps
      - FlightNumber
      - Origin
      - Destination
      - Date
      - CabinClass
  /operations/flightstatus/route/{origin}/{destination}/{date}:
    get:
      summary: Flight Status by Route
      description: Status of flights between a given origin and destination on a given
        date.
      operationId: OperationsFlightstatusRouteDateByOriginAndDestinationGet
      x-api-path-slug: operationsflightstatusrouteorigindestinationdate-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: date
        description: Departure date (YYYY-MM-DD) in local time of departure airport
      - in: path
        name: destination
        description: 3-letter IATA airport code (e
      - in: query
        name: limit
        description: Number of records returned per request
      - in: query
        name: offset
        description: Number of records skipped
      - in: path
        name: origin
        description: 3-letter IATA airport (e
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Flightstatus
      - Route
      - Origin
      - Destination
      - Date
  /operations/flightstatus/{flightNumber}/{date}:
    get:
      summary: Flight Status
      description: Status of a particular flight (boarding, delayed, etc.).
      operationId: OperationsFlightstatusByFlightNumberAndDateGet
      x-api-path-slug: operationsflightstatusflightnumberdate-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: date
        description: The departure date (YYYY-MM-DD) in the local time of the departure
          airport
      - in: path
        name: flightNumber
        description: Flight number including carrier code and any suffix (e
      - in: query
        name: limit
        description: Number of records returned per request
      - in: query
        name: offset
        description: Number of records skipped
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Flightstatus
      - FlightNumber
      - Date
---