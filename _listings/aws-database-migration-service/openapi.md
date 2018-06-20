---
swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 1
info:
  title: AWS Database Migration Service API
  version: 1.0.0
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
---