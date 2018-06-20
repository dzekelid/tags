---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateTags:
    get:
      summary: Create Tags
      description: |-
        Adds or overwrites one or more tags for the specified Amazon EC2 resource or
                 resources.
      operationId: createtags
      x-api-path-slug: actioncreatetags-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: ResourceId.N
        description: The ID of the resource
        type: string
      - in: query
        name: Tag.N
        description: One or more tags to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=DeleteTags:
    get:
      summary: Delete Tags
      description: Deletes the specified set of tags from the specified set of resources.
      operationId: deletetags
      x-api-path-slug: actiondeletetags-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return in a single call
        type: string
      - in: query
        name: NextToken
        description: The token to retrieve the next page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=DescribeTags:
    get:
      summary: Describe Tags
      description: Describes one or more of the tags for your EC2 resources.
      operationId: describetags
      x-api-path-slug: actiondescribetags-get
      parameters:
      - in: query
        name: ConversionTaskId
        description: The ID of the conversion task
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,      and provides an error response
        type: string
      - in: query
        name: ReasonMessage
        description: The reason for canceling the conversion task
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
---