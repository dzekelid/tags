swagger: "2.0"
x-collection-name: Google Tag Manager
x-complete: 1
info:
  title: Tag Manager
  description: accesses-tag-manager-accounts-and-containers-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tagmanager/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/containers/{containerId}/tags:
    get:
      summary: Get GTM Tags
      description: Lists all GTM Tags of a Container.
      operationId: tagmanager.accounts.containers.tags.list
      x-api-path-slug: accountsaccountidcontainerscontaineridtags-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Tag
    post:
      summary: Create GTM Tag
      description: Creates a GTM Tag.
      operationId: tagmanager.accounts.containers.tags.create
      x-api-path-slug: accountsaccountidcontainerscontaineridtags-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Tag
  /accounts/{accountId}/containers/{containerId}/tags/{tagId}:
    delete:
      summary: Delete GTM Tag
      description: Deletes a GTM Tag.
      operationId: tagmanager.accounts.containers.tags.delete
      x-api-path-slug: accountsaccountidcontainerscontaineridtagstagid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: tagId
        description: The GTM Tag ID
      responses:
        200:
          description: OK
      tags:
      - GTM Tag
    get:
      summary: Get GTM Tag
      description: Gets a GTM Tag.
      operationId: tagmanager.accounts.containers.tags.get
      x-api-path-slug: accountsaccountidcontainerscontaineridtagstagid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: tagId
        description: The GTM Tag ID
      responses:
        200:
          description: OK
      tags:
      - GTM Tag
    put:
      summary: Update GTM Tag
      description: Updates a GTM Tag.
      operationId: tagmanager.accounts.containers.tags.update
      x-api-path-slug: accountsaccountidcontainerscontaineridtagstagid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the tag in storage
      - in: path
        name: tagId
        description: The GTM Tag ID
      responses:
        200:
          description: OK
      tags:
      - GTM Tag