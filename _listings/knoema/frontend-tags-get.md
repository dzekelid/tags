---
swagger: "2.0"
info:
  title: Knoema API List of tags
  description: Lists out all the public tags present in the system
  version: 1.0.0
host: knoema.com
basePath: /api/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /frontend/tags:
    get:
      summary: List of tags
      description: Lists out all the public tags present in the system
      operationId: getTags
      responses:
        200:
          description: OK
      tags:
      - tags
definitions: []
x-collection-name: Knoema
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