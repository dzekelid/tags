---
swagger: "2.0"
x-collection-name: US Digital Registry
x-complete: 0
info:
  title: U.S. Digital Registry Tag API Tag Types
  description: This returns a tag based on an ID.
  version: 1.0.0
host: usdigitalregistry.digitalgov.gov
basePath: /api/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags/types.json:
    get:
      summary: Tag Types
      description: This returns a tag based on an ID.
      operationId: Api::V1::Tags#types
      x-api-path-slug: tagstypes-json-get
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