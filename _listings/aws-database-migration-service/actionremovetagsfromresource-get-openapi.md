---
swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 0
info:
  title: AWS Database Migration Service API Remove Tags From Resource
  version: 1.0.0
  description: Removes metadata tags from a DMS resource.
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
      description: Adds metadata tags to a DMS resource, including replication instance,
        endpoint, security group, and migration task.
      operationId: addTagsToResource
      x-api-path-slug: actionaddtagstoresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: The Amazon Resource Name (ARN) of the AWS DMS resource the tag
          is to be added to
        type: string
      - in: query
        name: Tags
        description: The tag to be assigned to the DMS resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Lists all tags for an AWS DMS resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the AWS DMS resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes metadata tags from a DMS resource.
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: '&gt;The Amazon Resource Name (ARN) of the AWS DMS resource the
          tag is to be removed from'
        type: string
      - in: query
        name: TagKeys
        description: The tag key (name) of the tag to be removed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
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