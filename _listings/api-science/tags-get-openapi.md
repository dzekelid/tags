---
swagger: "2.0"
x-collection-name: API Science
x-complete: 0
info:
  title: API Science List All Tags
  version: 1.0.0
  description: List All Tags
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags:
    get:
      summary: List All Tags
      description: List All Tags
      operationId: listAllTags
      x-api-path-slug: tags-get
      parameters:
      - in: query
        name: detailed
        description: Detailed List All Tags
      responses:
        200:
          description: OK
      tags:
      - Tags
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