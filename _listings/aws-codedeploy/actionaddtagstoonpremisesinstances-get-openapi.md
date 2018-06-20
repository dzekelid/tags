---
swagger: "2.0"
x-collection-name: AWS CodeDeploy
x-complete: 0
info:
  title: AWS CodeDeploy API Add Tags To On Premises Instances
  version: 1.0.0
  description: Adds tags to on-premises instances.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddTagsToOnPremisesInstances:
    get:
      summary: Add Tags To On Premises Instances
      description: Adds tags to on-premises instances.
      operationId: addTagsToOnPremisesInstances
      x-api-path-slug: actionaddtagstoonpremisesinstances-get
      parameters:
      - in: query
        name: instanceNames
        description: The names of the on-premises instances to which to add tags
        type: string
      - in: query
        name: tags
        description: The tag key-value pairs to add to the on-premises instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Premises Instances Tags
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