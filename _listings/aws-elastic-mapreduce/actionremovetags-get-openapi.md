---
swagger: "2.0"
x-collection-name: AWS Elastic MapReduce
x-complete: 0
info:
  title: AWS Elastic MapReduce API Remove Tags
  version: 1.0.0
  description: Removes tags from an Amazon EMR resource.
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
      description: Adds tags to an Amazon EMR resource.
      operationId: addTags
      x-api-path-slug: actionaddtags-get
      parameters:
      - in: query
        name: ResourceId
        description: The Amazon EMR resource identifier to which tags will be added
        type: string
      - in: query
        name: Tags
        description: A list of tags to associate with a cluster and propagate to EC2
          instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=RemoveTags:
    get:
      summary: Remove Tags
      description: Removes tags from an Amazon EMR resource.
      operationId: removeTags
      x-api-path-slug: actionremovetags-get
      parameters:
      - in: query
        name: ResourceId
        description: The Amazon EMR resource identifier from which tags will be removed
        type: string
      - in: query
        name: TagKeys
        description: A list of tag keys to remove from a resource
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