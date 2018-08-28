---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Remove Tags From Resource
  version: 1.0.0
  description: Removes metadata tags from an Amazon RDS resource.
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
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Lists all tags on an Amazon RDS resource.
      operationId: listtagsforresource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: ResourceName
        description: The Amazon RDS resource with tags to be listed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes metadata tags from an Amazon RDS resource.
      operationId: removetagsfromresource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceName
        description: The Amazon RDS resource the tags will be removed from
        type: string
      - in: query
        name: TagKeys.member.N
        description: The tag key (name) of the tag to be removed
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