---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 0
info:
  title: AWS S3 GET Object tagging
  version: 1.0.0
  description: This implementation of the GET operation returns the tags associated
    with anobject
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?tagging:
    delete:
      summary: DELETE Bucket tagging
      description: This implementation of the DELETE operation uses the taggingsubresource
        to remove a tag set from the specified bucket
      operationId: delete-bucket-tagging
      x-api-path-slug: tagging-delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Tagging
    get:
      summary: GET Bucket tagging
      description: This implementation of the GET operation uses the taggingsubresource
        to return the tag set associated with the bucket
      operationId: get-bucket-tagging
      x-api-path-slug: tagging-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Tagging
    put:
      summary: PUT Bucket tagging
      description: This implementation of the PUT operation uses the taggingsubresource
        to add a set of tags to an existing bucket
      operationId: put-bucket-tagging
      x-api-path-slug: tagging-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Tagging
  /ObjectName?tagging:
    get:
      summary: GET Object tagging
      description: This implementation of the GET operation returns the tags associated
        with anobject
      operationId: get-object-tagging
      x-api-path-slug: objectnametagging-get
      responses:
        200:
          description: OK
      tags:
      - Object
      - Tagging
    put:
      summary: PUT Object tagging
      description: This implementation of the PUT operation uses the taggingsubresource
        to add a set of tags to an existing object
      operationId: put-object-tagging
      x-api-path-slug: objectnametagging-put
      responses:
        200:
          description: OK
      tags:
      - Object
      - Tagging
  ObjectKey/?tagging:
    delete:
      summary: DELETE Object tagging
      description: This implementation of the DELETE operation uses thetagging subresource
        to remove the entire tag set from thespecified object
      operationId: delete-object-tagging
      x-api-path-slug: objectkeytagging-delete
      responses:
        200:
          description: OK
      tags:
      - Object
      - Tagging
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