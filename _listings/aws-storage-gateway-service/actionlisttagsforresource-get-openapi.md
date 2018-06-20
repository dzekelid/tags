---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 0
info:
  title: AWS Storage Gateway Service API List Tags For Resource
  version: 1.0.0
  description: Lists the tags that have been added to the specified resource.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddTagsToResource:
    get:
      summary: Add Tags To Resource
      description: Adds one or more tags to the specified resource.
      operationId: addTagsToResource
      x-api-path-slug: actionaddtagstoresource-get
      parameters:
      - in: query
        name: ResourceARN
        description: The Amazon Resource Name (ARN) of the resource you want to add
          tags to
        type: string
      - in: query
        name: Tags
        description: The key-value pair that represents the tag you want to add to
          the resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Lists the tags that have been added to the specified resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: Limit
        description: Specifies that the list of tags returned be limited to the specified
          number of         items
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          returning the list of         tags
        type: string
      - in: query
        name: ResourceARN
        description: The Amazon Resource Name (ARN) of the resource for which you
          want to list         tags
        type: string
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