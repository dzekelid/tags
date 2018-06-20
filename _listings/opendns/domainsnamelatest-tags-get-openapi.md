---
swagger: "2.0"
x-collection-name: OpenDNS
x-complete: 0
info:
  title: OpenDNS Tagging
  version: 1.0.0
  description: This endpoint returns the date range when the domain being queried
    was a part of the OpenDNS block list. A common use case is to find how long a
    domain has been in the block list for domains being blocked currently. However
    it will also show a record of the history of the domain in the OpenDNS blocklis
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /domains/{name}/latest_tags:
    get:
      summary: Tagging
      description: This endpoint returns the date range when the domain being queried
        was a part of the OpenDNS block list. A common use case is to find how long
        a domain has been in the block list for domains being blocked currently. However
        it will also show a record of the history of the domain in the OpenDNS blocklis
      operationId: domainTagging
      x-api-path-slug: domainsnamelatest-tags-get
      parameters:
      - in: path
        name: Domain Name
        description: Domain Name
        type: string
        format: string
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