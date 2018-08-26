---
swagger: "2.0"
x-collection-name: Fire Browse
x-complete: 1
info:
  title: Fire Browse Beta API
  description: a-simple-and-elegant-way-to-explore-cancer-data
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
---