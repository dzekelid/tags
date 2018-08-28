---
swagger: "2.0"
x-collection-name: Azure Resource Manager
x-complete: 0
info:
  title: Azure Resource Manager API Tags Delete Value
  description: Deletes a tag value.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/tagNames/{tagName}/tagValues/{tagValue}:
    delete:
      summary: Tags Delete Value
      description: Deletes a tag value.
      operationId: Tags_DeleteValue
      x-api-path-slug: subscriptionssubscriptionidtagnamestagnametagvaluestagvalue-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: tagName
        description: The name of the tag
      - in: path
        name: tagValue
        description: The value of the tag to delete
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