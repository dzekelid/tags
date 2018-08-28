---
swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 0
info:
  title: HPE OneSphere API Get Tags
  description: Returns a tag based on its id. It requires the **consumer** global
    role.
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
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
      description: Lists tags.
      operationId: ListTags
      x-api-path-slug: tags-get
      parameters:
      - in: query
        name: view
        description: 'Return related resources:  * `full` - include each tags related
          `tag-key`'
      responses:
        200:
          description: OK
      tags:
      - Tags
    post:
      summary: Post Tags
      description: Create a tag. It requires the **analyst** global role.
      operationId: CreateTag
      x-api-path-slug: tags-post
      parameters:
      - in: body
        name: tag
        description: New tag
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/{id}:
    delete:
      summary: Delete Tags
      description: Delete a tag. It requires the **analyst** global role.
      operationId: DeleteTag
      x-api-path-slug: tagsid-delete
      parameters:
      - in: path
        name: id
        description: ID of tag to delete
      responses:
        200:
          description: OK
      tags:
      - Tags
    get:
      summary: Get Tags
      description: Returns a tag based on its id. It requires the **consumer** global
        role.
      operationId: GetTagById
      x-api-path-slug: tagsid-get
      parameters:
      - in: path
        name: id
        description: ID of tag to fetch
      - in: query
        name: view
        description: 'Return related resources:  * `full` - Include the tags related
          `tag-key`'
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