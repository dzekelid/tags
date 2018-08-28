---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Admin Place Tags Main
  version: 1.0.0
  description: Get admin place tags main.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/admin/event/tags/main:
    get:
      summary: Get Admin Event Tags Main
      description: Get admin event tags main.
      operationId: getApiV1AdminEventTagsMain
      x-api-path-slug: apiv1admineventtagsmain-get
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Tags
      - Main
  /api/v1/admin/event/tags/additional:
    get:
      summary: Get Admin Event Tags Additional
      description: Get admin event tags additional.
      operationId: getApiV1AdminEventTagsAdditional
      x-api-path-slug: apiv1admineventtagsadditional-get
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Tags
      - Itional
  /api/v1/admin/place/tags/main:
    get:
      summary: Get Admin Place Tags Main
      description: Get admin place tags main.
      operationId: getApiV1AdminPlaceTagsMain
      x-api-path-slug: apiv1adminplacetagsmain-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Tags
      - Main
  /api/v1/admin/place/tags/additional:
    get:
      summary: Get Admin Place Tags Additional
      description: Get admin place tags additional.
      operationId: getApiV1AdminPlaceTagsAdditional
      x-api-path-slug: apiv1adminplacetagsadditional-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Tags
      - Itional
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