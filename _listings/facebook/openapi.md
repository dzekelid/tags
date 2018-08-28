swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{photo}/tags:
    get:
      summary: Get Photo Tags
      description: Tags for this photo.
      operationId: getPhotoTags
      x-api-path-slug: phototags-get
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Tags
    post:
      summary: Post Photo Tags
      description: Creates a tag on this photo.
      operationId: postPhotoTags
      x-api-path-slug: phototags-post
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      - in: query
        name: to
        description: USER_ID of the User to tag; can also be provided in URL path
      - in: query
        name: x
        description: x coordinate of tag, as a percentage offset from the left edge
          of the picture
      - in: query
        name: "y"
        description: y coordinate of tag, as a percentage offset from the top edge
          of the picture
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Tags
  /{photo}/tags/{user}:
    post:
      summary: Post Photo Tags User
      description: Updates the position of a tag on this photo for the user.
      operationId: postPhotoTagsUser
      x-api-path-slug: phototagsuser-post
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      - in: path
        name: user
        description: Represents the ID of the user
      - in: query
        name: x
        description: x coordinate of tag, as a percentage offset from the left edge
          of the picture
      - in: query
        name: "y"
        description: y coordinate of tag, as a percentage offset from the top edge
          of the picture
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Tags
      - User
  /{application}/tagged:
    get:
      summary: Get Application Tagged
      description: The photos, videos, and posts in which this application has been
        tagged.
      operationId: getApplicationTagged
      x-api-path-slug: applicationtagged-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Tagged
  /{page}/tagged:
    get:
      summary: Get Page Tagged
      description: The photos, videos, and posts in which this page has been tagged
      operationId: getPageTagged
      x-api-path-slug: pagetagged-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Tagged
  /{user}/tagged:
    get:
      summary: Get User Tagged
      description: Posts the user is tagged in
      operationId: getUserTagged
      x-api-path-slug: usertagged-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Tagged