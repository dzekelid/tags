---
swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 0
info:
  title: AWS Auto Scaling API Describe Tags
  version: 1.0.0
  description: Describes the specified tags.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateOrUpdateTags:
    get:
      summary: Create Or Update Tags
      description: Creates or updates tags for the specified Auto Scaling group.
      operationId: createOrUpdateTags
      x-api-path-slug: actioncreateorupdatetags-get
      parameters:
      - in: query
        name: Tags.member.N
        description: One or more tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=DeleteTags:
    get:
      summary: Delete Tags
      description: Deletes the specified tags.
      operationId: deleteTags
      x-api-path-slug: actiondeletetags-get
      parameters:
      - in: query
        name: Tags.member.N
        description: One or more tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=DescribeTags:
    get:
      summary: Describe Tags
      description: Describes the specified tags.
      operationId: describeTags
      x-api-path-slug: actiondescribetags-get
      parameters:
      - in: query
        name: Filters.member.N
        description: A filter used to scope the tags to return
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
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