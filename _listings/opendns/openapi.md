swagger: "2.0"
x-collection-name: OpenDNS
x-complete: 1
info:
  title: OpenDNS
  version: 1.0.0
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