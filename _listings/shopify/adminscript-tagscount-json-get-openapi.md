---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Get a count of all script tags
  description: Get a count of all script tags.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/articles/tags.json:
    get:
      summary: Get a list of all the tags of articles
      description: Get a list of all the tags of articles.
      operationId: getAdminArticlesTags.json
      x-api-path-slug: adminarticlestags-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Tags
      - Articles
  /admin/blogs/62581763/articles/197247246.json:
    delete:
      summary: Delete an article of a blog tags of articles
      description: Delete an article of a blog tags of articles.
      operationId: deleteAdminBlogs62581763Articles197247246.json
      x-api-path-slug: adminblogs62581763articles197247246-json-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Article
      - Blog
      - Tags
      - Articles
  /admin/script_tags.json:
    get:
      summary: Get a list of all script tags
      description: Get a list of all script tags.
      operationId: getAdminScriptTags.json
      x-api-path-slug: adminscript-tags-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Script
      - Tags
  /admin/script_tags/count.json:
    get:
      summary: Get a count of all script tags
      description: Get a count of all script tags.
      operationId: getAdminScriptTagsCount.json
      x-api-path-slug: adminscript-tagscount-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Count
      - Script
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