---
swagger: "2.0"
x-collection-name: Datadog
x-complete: 0
info:
  title: DataDog API Get Tags Hosts
  version: 1.0.0
  description: Return a mapping of tags to hosts for your whole infrastructure.
basePath: api/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags/hosts:
    get:
      summary: Get Tags Hosts
      description: Return a mapping of tags to hosts for your whole infrastructure.
      operationId: getTagsHosts
      x-api-path-slug: tagshosts-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tags
      - Hosts
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