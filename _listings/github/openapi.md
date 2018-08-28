swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repos/{owner}/{repo}/git/tags:
    post:
      summary: Add Repos Owner Repo Git Tags
      description: |-
        Create a Tag Object.
        Note that creating a tag object does not create the reference that makes a
        tag in Git. If you want to create an annotated tag in Git, you have to do
        this call to create the tag object, and then create the refs/tags/[tag]
        reference. If you want to create a lightweight tag, you only have to create
        the tag reference - this call would be unnecessary.
      operationId: create-a-tag-objectnote-that-creating-a-tag-object-does-not-create-the-reference-that-makes-atag-in-
      x-api-path-slug: reposownerrepogittags-post
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Git
      - Tags
  /repos/{owner}/{repo}/git/tags/{shaCode}:
    get:
      summary: Get Repos Owner Repo Git Tags Shacode
      description: Get a Tag.
      operationId: get-a-tag
      x-api-path-slug: reposownerrepogittagsshacode-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      - in: path
        name: shaCode
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Git
      - Tags
      - Shacode
  /repos/{owner}/{repo}/tags:
    get:
      summary: Get Repos Owner Repo Tags
      description: Get list of tags.
      operationId: get-list-of-tags
      x-api-path-slug: reposownerrepotags-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Tags