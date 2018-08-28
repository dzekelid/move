---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Move screen tab
  description: Moves tab position
  termsOfService: http://atlassian.com/terms/
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