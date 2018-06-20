---
swagger: "2.0"
x-collection-name: AWS Elastic Load Balancing
x-complete: 0
info:
  title: AWS Elastic Load Balancing API Add Tags
  version: 1.0.0
  description: Adds the specified tags to the specified resource.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddTags:
    get:
      summary: Add Tags
      description: Adds the specified tags to the specified resource.
      operationId: addTags
      x-api-path-slug: actionaddtags-get
      parameters:
      - in: query
        name: ResourceArns.member.N
        description: The Amazon Resource Name (ARN) of the resource
        type: string
      - in: query
        name: Tags.member.N
        description: The tags
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