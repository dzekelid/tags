---
swagger: "2.0"
x-collection-name: DigitalOcean
x-complete: 0
info:
  title: Digital Ocean List all Tags
  description: "To list all of your tags, you can send a GET request to /v2/tags.\r\n\r\nThe
    response will be a JSON object with a key called _tags_."
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags:
    get:
      summary: List all Tags
      description: "To list all of your tags, you can send a GET request to /v2/tags.\r\n\r\nThe
        response will be a JSON object with a key called _tags_."
      operationId: TagsGet
      x-api-path-slug: tags-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
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