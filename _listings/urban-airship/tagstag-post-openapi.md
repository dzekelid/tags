---
swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 0
info:
  title: Urban Airship Post Tags Tag
  description: Modifies device tokens on a tag.
  version: v3
host: go.urbanairship.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags:
    get:
      summary: Get Tags
      description: Returns all the tags that you have created.
      operationId: tags.get
      x-api-path-slug: tags-get
      parameters:
      - in: query
        name: feed_id
        description: A particular feed
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/{tag}:
    put:
      summary: Put Tags Tag
      description: Deletes a tag.
      operationId: tags.tag.put
      x-api-path-slug: tagstag-put
      parameters:
      - in: query
        name: tag
        description: Tags can be of any format you wish, but we recommend that they
          be URL-safe in order to make less work for you
      - in: path
        name: tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Tag
    post:
      summary: Post Tags Tag
      description: Modifies device tokens on a tag.
      operationId: tags.tag.post
      x-api-path-slug: tagstag-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: tag
        description: Tags can be of any format you wish, but we recommend that they
          be URL-safe in order to make less work for you
      - in: path
        name: tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Tag
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