---
swagger: "2.0"
x-collection-name: AWS Elasticsearch Service
x-complete: 0
info:
  title: Amazon Elasticsearch Service API Add Tags
  version: 1.0.0
  description: |-
    Attaches resource tags to an Amazon ES domain. Use the POST HTTP method
                    with this operation. For more information, see Tagging Amazon ES
                    Domains.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2015-01-01/tags:
    post:
      summary: Add Tags
      description: |-
        Attaches resource tags to an Amazon ES domain. Use the POST HTTP method
                        with this operation. For more information, see Tagging Amazon ES
                        Domains.
      operationId: addTags
      x-api-path-slug: 20150101tags-post
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