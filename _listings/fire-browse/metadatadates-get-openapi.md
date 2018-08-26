---
swagger: "2.0"
x-collection-name: Fire Browse
x-complete: 0
info:
  title: Fire Browse Beta API Retrieve datestamps of all GDAC Firehose standard data
    and analyses runs that have been ingested into FireBrowse.
  description: Retrieve datestamps of all gdac firehose standard data and analyses
    runs that have been ingested into firebrowse..
  version: 1.1.35 (2016-09-27 10:12:23 6a47e74011281b2aa
host: firebrowse.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Metadata/Dates:
    get:
      summary: Retrieve datestamps of all GDAC Firehose standard data and analyses
        runs that have been ingested into FireBrowse.
      description: Retrieve datestamps of all gdac firehose standard data and analyses
        runs that have been ingested into firebrowse..
      operationId: getMetadataDates
      x-api-path-slug: metadatadates-get
      parameters:
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Dates
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