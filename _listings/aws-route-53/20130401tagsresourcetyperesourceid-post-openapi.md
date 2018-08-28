---
swagger: "2.0"
x-collection-name: AWS Route 53
x-complete: 0
info:
  title: AWS Route 53 API Change Tags For Resource
  version: 1.0.0
  description: Adds, edits, or deletes tags for a health check or a hosted zone.For
    information about using tags for cost allocation, see Using Cost Allocation Tags
    in the AWS Billing and Cost Management User Guide.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2013-04-01/tags/ResourceType/ResourceId:
    get:
      summary: List Tags For Resource
      description: Lists tags for one health check or hosted zone. For information
        about using tags for cost allocation, see Using Cost Allocation Tags in the
        AWS Billing and Cost Management User Guide.
      operationId: listtagsforresource
      x-api-path-slug: 20130401tagsresourcetyperesourceid-get
      parameters:
      - in: path
        name: ResourceId
        description: The ID of the resource for which you want to retrieve tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
    post:
      summary: Change Tags For Resource
      description: Adds, edits, or deletes tags for a health check or a hosted zone.For
        information about using tags for cost allocation, see Using Cost Allocation
        Tags in the AWS Billing and Cost Management User Guide.
      operationId: changetagsforresource
      x-api-path-slug: 20130401tagsresourcetyperesourceid-post
      parameters:
      - in: body
        name: AddTags
        description: A complex type that contains a list of the tags that you want
          to add to the specifiedhealth check or hosted zone and/or the tags for which
          you want to edit the Valueelement
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: ChangeTagsForResourceRequest
        description: Root level tag for the ChangeTagsForResourceRequest parameters
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: RemoveTagKeys
        description: A complex type that contains a list of the tags that you want
          to delete from thespecified health check or hosted zone
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: ResourceId
        description: The ID of the resource for which you want to add, change, or
          delete tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Changes
  /2013-04-01/tags/ResourceType:
    post:
      summary: List Tags For Resources
      description: Lists tags for up to 10 health checks or hosted zones.For information
        about using tags for cost allocation, see Using Cost Allocation Tags in the
        AWS Billing and Cost Management User Guide.
      operationId: listtagsforresources
      x-api-path-slug: 20130401tagsresourcetype-post
      parameters:
      - in: body
        name: ListTagsForResourcesRequest
        description: Root level tag for the ListTagsForResourcesRequest parameters
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: ResourceIds
        description: A complex type that contains the ResourceId element for each
          resource for which youwant to get a list of tags
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: ResourceType
        description: The type of the resources
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