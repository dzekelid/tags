---
swagger: "2.0"
x-collection-name: AWS Route 53
x-complete: 0
info:
  title: AWS Route 53 API List Tags For Resource
  version: 1.0.0
  description: Lists tags for one health check or hosted zone. For information about
    using tags for cost allocation, see Using Cost Allocation Tags in the AWS Billing
    and Cost Management User Guide.
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