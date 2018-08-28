swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/screens/{screenId}/tabs/{tabId}/fields/{id}/move:
    post:
      summary: Move screen tab field
      description: Moves field on the given tab
      operationId: com.atlassian.jira.rest.v2.issue.ScreensResource.moveScreenTabField_post
      x-api-path-slug: api2screensscreenidtabstabidfieldsidmove-post
      parameters:
      - in: path
        name: id
      - in: path
        name: screenId
        description: id of screen
      - in: path
        name: tabId
        description: id of tab
      responses:
        200:
          description: OK
      tags:
      - Move
      - Screen
      - Tab
      - Field
  /api/2/screens/{screenId}/tabs/{tabId}/move/{pos}:
    post:
      summary: Move screen tab
      description: Moves tab position
      operationId: com.atlassian.jira.rest.v2.issue.ScreensResource.moveScreenTab_post
      x-api-path-slug: api2screensscreenidtabstabidmovepos-post
      parameters:
      - in: path
        name: pos
        description: position of tab
      - in: path
        name: screenId
        description: id of screen
      - in: path
        name: tabId
        description: id of tab
      responses:
        200:
          description: OK
      tags:
      - Move
      - Screen
      - Tab
  /api/2/version/{id}/move:
    post:
      summary: Move version
      description: Modifies the version's sequence within the project, which affects
        the display order of the versions in Jira. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg)
        or _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.moveVersion_post
      x-api-path-slug: api2versionidmove-post
      parameters:
      - in: path
        name: id
        description: The ID of the version to be moved
      responses:
        200:
          description: OK
      tags:
      - Move
      - Version