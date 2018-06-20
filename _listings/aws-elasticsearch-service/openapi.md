---
swagger: "2.0"
x-collection-name: AWS Elasticsearch Service
x-complete: 1
info:
  title: AWS Elasticsearch Service API
  version: 1.0.0
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
  /2015-01-01/tags?arn={domain_arn}:
    get:
      summary: List Tags
      description: |-
        Displays all of the tags for an Amazon ES domain. Use the GET HTTP method
                        with this operation.
      operationId: listTags
      x-api-path-slug: 20150101tagsarndomain-arn-get
      responses:
        200:
          description: OK
      tags:
      - Tags
  es.{aws_region}.amazonaws.com/2015-01-01/tags-removal:
    post:
      summary: Remove Tags
      description: |-
        Removes the specified resource tags from an Amazon ES domain. Use the POST
                        HTTP method with this operation.
      operationId: removeTags
      x-api-path-slug: es-aws-region-amazonaws-com20150101tagsremoval-post
      responses:
        200:
          description: OK
      tags:
      - Tags
---