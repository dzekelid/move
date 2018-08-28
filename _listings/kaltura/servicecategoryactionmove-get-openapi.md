---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 0
info:
  title: Kaltura VPaaS Get Service Category Action Move
  description: Move categories that belong to the same parent category to a target
    categroy - enabled only for ks with disable entitlement
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/category/action/move:
    get:
      summary: Get Service Category Action Move
      description: Move categories that belong to the same parent category to a target
        categroy - enabled only for ks with disable entitlement
      operationId: category.move
      x-api-path-slug: servicecategoryactionmove-get
      parameters:
      - in: query
        name: categoryIds
      - in: query
        name: No Name
      - in: query
        name: targetCategoryParentId
      responses:
        200:
          description: OK
      tags:
      - Service
      - Category
      - Action
      - Move
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