swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 1
info:
  title: Bitbucket
  description: code-against-the-bitbucket-api-to-automate-simple-tasks-embed-bitbucket-data-into-your-own-site-build-mobile-or-desktop-apps-or-even-add-custom-ui-addons-into-bitbucket-itself-using-the-connect-framework-
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repositories/{username}/{repo_slug}/refs/tags:
    get:
      summary: Get Repositories Username Repo Slug Refs Tags
      description: Get repositories username repo slug refs tags
      operationId: getRepositoriesUsernameRepoSlugRefsTags
      x-api-path-slug: repositoriesusernamerepo-slugrefstags-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Refs
      - Tags
    parameters:
      summary: Parameters Repositories Username Repo Slug Refs Tags
      description: Parameters repositories username repo slug refs tags
      operationId: parametersRepositoriesUsernameRepoSlugRefsTags
      x-api-path-slug: repositoriesusernamerepo-slugrefstags-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Refs
      - Tags
    post:
      summary: Add Repositories Username Repo Slug Refs Tags
      description: |-
        Creates a new tag in the specified repository.

        The payload of the POST should consist of a JSON document that
        contains the name of the tag and the target hash.

        ```
        {
            "name" : "new tag name",
            "target" : {
                "hash" : "target commit hash",
            }
        }
        ```

        This endpoint does support using short hash prefixes for the commit
        hash, but it may return a 400 response if the provided prefix is
        ambiguous. Using a full commit hash is the preferred approach.
      operationId: postRepositoriesUsernameRepoSlugRefsTags
      x-api-path-slug: repositoriesusernamerepo-slugrefstags-post
      parameters:
      - in: body
        name: _body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Refs
      - Tags
  /repositories/{username}/{repo_slug}/refs/tags/{name}:
    get:
      summary: Get Repositories Username Repo Slug Refs Tags Name
      description: Get repositories username repo slug refs tags name
      operationId: getRepositoriesUsernameRepoSlugRefsTagsName
      x-api-path-slug: repositoriesusernamerepo-slugrefstagsname-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Refs
      - Tags
      - Name
    parameters:
      summary: Parameters Repositories Username Repo Slug Refs Tags Name
      description: Parameters repositories username repo slug refs tags name
      operationId: parametersRepositoriesUsernameRepoSlugRefsTagsName
      x-api-path-slug: repositoriesusernamerepo-slugrefstagsname-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Refs
      - Tags
      - Name