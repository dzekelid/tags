---
swagger: "2.0"
x-collection-name: Pinboard
x-complete: 0
info:
  title: Pinboard Deletes Tag
  description: Delete an existing tag.
  version: 1.0.0
host: api.pinboard.in
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags/get:
    get:
      summary: Get Tags
      description: Returns a full list of the user's tags along with the number of
        times they were used.
      operationId: tags.get.get
      x-api-path-slug: tagsget-get
      parameters:
      - in: query
        name: format
        description: the format to return
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/delete:
    get:
      summary: Deletes Tag
      description: Delete an existing tag.
      operationId: tags.delete.get
      x-api-path-slug: tagsdelete-get
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