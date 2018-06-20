---
swagger: "2.0"
x-collection-name: AWS CloudHSM
x-complete: 0
info:
  title: AWS CloudHSM API Remove Tags From Resource
  version: 1.0.0
  description: Removes one or more tags from the specified AWS CloudHSM resource.
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
      description: Adds or overwrites one or more tags for the specified AWS CloudHSM
        resource.
      operationId: addTagsToResource
      x-api-path-slug: actionaddtagstoresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: The Amazon Resource Name (ARN) of the AWS CloudHSM resource to
          tag
        type: string
      - in: query
        name: TagList
        description: One or more tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Returns a list of all tags for the specified AWS CloudHSM resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: The Amazon Resource Name (ARN) of the AWS CloudHSM resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes one or more tags from the specified AWS CloudHSM resource.
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: The Amazon Resource Name (ARN) of the AWS CloudHSM resource
        type: string
      - in: query
        name: TagKeyList
        description: The tag key or keys to remove
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