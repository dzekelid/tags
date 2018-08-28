---
swagger: "2.0"
x-collection-name: 500px
x-complete: 0
info:
  title: 500px Delete Photos Tags
  description: Removes tags from the photo. Accepts one or multiple coma separated
    tags.
  version: v1
host: api.500px.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /photos/:id/tags:
    delete:
      summary: Delete Photos Tags
      description: Removes tags from the photo. Accepts one or multiple coma separated
        tags.
      operationId: deletePhotosTags
      x-api-path-slug: photosidtags-delete
      parameters:
      - in: query
        name: id (required)
        description: The Photo ID to remove tags from
      - in: query
        name: tags (required)
        description: Coma separated tags
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Tags
    post:
      summary: Post Photos Tags
      description: Adds tags to the photo. Accepts one or multiple coma separated
        tags.
      operationId: postPhotosTags
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
      - Tags
  /photos/{id}/tags:
    post:
      summary: Post Photos Tags
      description: Adds tags to the photo. Accepts one or multiple coma separated
        tags.
      operationId: postPhotosTags
      x-api-path-slug: photosidtags-post
      parameters:
      - in: path
        name: id
        description: The Photo ID to add tags for
      - in: query
        name: tags
        description: Coma separated tags
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Tags
    delete:
      summary: Delete Photos Tags
      description: Removes tags from the photo. Accepts one or multiple coma separated
        tags.
      operationId: deletePhotosTags
      x-api-path-slug: photosidtags-delete
      parameters:
      - in: path
        name: id
        description: The Photo ID to remove tags from
      - in: query
        name: tags
        description: Coma separated tags
      responses:
        200:
          description: OK
      tags:
      - Photos
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