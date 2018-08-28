swagger: "2.0"
x-collection-name: Mailgun
x-complete: 1
info:
  title: Mailgun API
  description: powerful-apis-that-allow-you-to-send-receive-and-track-email-effortlessly-
  version: v2
host: api.mailgun.net
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  tags/{tag}:
    delete:
      summary: Delete Tag
      description: Deletes all counters for particular tag and the tag itself.
      operationId: deleteTagsTag
      x-api-path-slug: tagstag-delete
      responses:
        200:
          description: OK
      tags:
      - Tag