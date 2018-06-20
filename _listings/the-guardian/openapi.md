---
swagger: "2.0"
x-collection-name: The Guardian
x-complete: 1
info:
  title: The Guardian
  description: the-guardian-content-api-is-a-public-service-for-accessing-all-the-content-the-guardian-creates-and-the-collections-we-have-of-that-content-tags-and-sections--there-are-over-one-and-a-half-million-items-available-published-as-far-back-as-1999--this-overview-will-give-you-some-idea-of-what-data-is-available-how-to-find-what-you-need-and-what-you-will-see-when-you-make-a-request-to-us-
  version: v1
host: content.guardianapis.com
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
      description: Retrieves the tags used across the Guardian news platform.
      operationId: tags
      x-api-path-slug: tags-get
      responses:
        200:
          description: OK
      tags:
      - Tags
---