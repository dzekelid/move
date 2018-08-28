---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Move widget onto another dashboard
  version: 1.0.0
  description: Move widget onto another dashboard.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/dashboard/movewidget:
    put:
      summary: Move widget onto another dashboard
      description: Move widget onto another dashboard.
      operationId: Dashboard_MoveWidgetBydataContract
      x-api-path-slug: apidashboardmovewidget-put
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Move
      - Widget
      - Onto
      - Another
      - Dashboard
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