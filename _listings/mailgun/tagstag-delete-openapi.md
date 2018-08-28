---
swagger: "2.0"
x-collection-name: Mailgun
x-complete: 0
info:
  title: Mailgun API Delete Tag
  description: Deletes all counters for particular tag and the tag itself.
  version: v2
host: api.mailgun.net
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  tags/{tag}:
    delete:
      summary: Delete Tag
      description: Deletes all counters for particular tag and the tag itself.
      operationId: deleteTagsTag
      x-api-path-slug: tagstag-delete
      responses:
        200:
          description: OK
      tags:
      - Tag
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