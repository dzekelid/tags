---
swagger: "2.0"
x-collection-name: Sustainable Facilities Tool API
x-complete: 1
info:
  title: Sustainable Facilities Tool API
  description: our-core-api-allows-developers-to-interact-with-the-sustainable-facilities-tool-programmatically--its-designed-for-public-use-and-to-be-easily-integrated-into-other-applications-
  termsOfService: https://sftool.gov/developer/terms-of-use
  version: 1.0.0
host: api.data.gov
basePath: /sftool/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags:
    get:
      summary: Tags
      description: Returns all search tags.
      operationId: getTags
      x-api-path-slug: tags-get
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/{parameter}:
    get:
      summary: Tag
      description: Returns a tag by parameter.
      operationId: getTag
      x-api-path-slug: tagsparameter-get
      responses:
        200:
          description: OK
      tags:
      - Tags
---