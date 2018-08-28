swagger: "2.0"
x-collection-name: AngelList
x-complete: 1
info:
  title: AngelList
  description: the-angellist-api-provides-developers-with-a-restful-interface-to-the-angellist-data-set--for-more-information-read-the-oauth-faq-
  termsOfService: https://angel.co/terms
  contact:
    name: AngelList
    url: https://angel.co/api
    email: api@angel.co
  version: v1
host: api.angel.co
basePath: /1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags/{tag_id}:
    get:
      summary: Get Tag
      description: Get Tag
      operationId: tags
      x-api-path-slug: tagstag-id-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
  /tags/{tag_id}/children:
    get:
      summary: Get Tags Children
      description: Get Tags Children
      operationId: tagsChildren
      x-api-path-slug: tagstag-idchildren-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
  /tags/{tag_id}/jobs:
    get:
      summary: Get Jobs by Tag
      description: Get Jobs by Tag
      operationId: jobs
      x-api-path-slug: tagstag-idjobs-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
  /tags/{tag_id}/parents:
    get:
      summary: Get Tag Parents
      description: Get Tag Parents
      operationId: tagParents
      x-api-path-slug: tagstag-idparents-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
  /tags/{tag_id}/startups:
    get:
      summary: Get Startups by Tag
      description: Get Startups by Tag
      operationId: tagStartups
      x-api-path-slug: tagstag-idstartups-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
  /tags/{tag_id}/users:
    get:
      summary: Get Users by Tag
      description: Get Users by Tag
      operationId: tagUsers
      x-api-path-slug: tagstag-idusers-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
      - Users