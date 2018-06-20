---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Post Photos Tags
  description: Adds tags to the photo. Accepts one or multiple coma separated tags.
  version: 1.0.0
host: /account
basePath: https://codenvy.com/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /photos/:id/tags:
    post:
      summary: Post Photos Tags
      description: Adds tags to the photo. Accepts one or multiple coma separated
        tags.
      operationId: adds-tags-to-the-photo-accepts-one-or-multiple-coma-separated-tags
      x-api-path-slug: photosidtags-post
      parameters:
      - in: query
        name: id (required)
        description: The Photo ID to add tags for
      - in: query
        name: tags (required)
        description: Coma separated tags
      responses:
        200:
          description: OK
      tags:
      - Photos
      - :id
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