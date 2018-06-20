---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Add Tags To Resource
  version: 1.0.0
  description: Adds metadata tags to an Amazon RDS resource.
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
      description: Adds metadata tags to an Amazon RDS resource.
      operationId: addtagstoresource
      x-api-path-slug: actionaddtagstoresource-get
      parameters:
      - in: query
        name: ResourceName
        description: The Amazon RDS resource the tags will be added to
        type: string
      - in: query
        name: Tags.Tag.N
        description: The tags to be assigned to the Amazon RDS resource
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