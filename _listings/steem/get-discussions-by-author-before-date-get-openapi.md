---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem get_discussions_by_author_before_date
  description: get_discussions_by_author_before_date
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_discussions_by_author_before_date:
    get:
      summary: get_discussions_by_author_before_date
      description: get_discussions_by_author_before_date
      operationId: get-discussions-by-author-before-date
      x-api-path-slug: get-discussions-by-author-before-date-get
      parameters:
      - in: query
        name: author
        description: account name
      - in: query
        name: beforeDate
        description: date and time
      - in: query
        name: limit
        description: limit query
      - in: query
        name: startPermlink
        description: permlink of post
      responses:
        200:
          description: OK
      tags:
      - Get
      - Discussions
      - By
      - Author
      - Before
      - Date
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