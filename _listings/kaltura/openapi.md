---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 1
info:
  title: Kaltura VPaaS
  description: building-video-experiences-consists-of-ingesting-media-files-playing-back-videos-and-reviewing-usage-and-engagement-analytics--in-between-there-is-a-world-of-nuances-required-for-your-unique-usecase-and-application--kaltura-vpaas-is-built-on-the-principles-of-atomic-services-sdks-and-tools-that-allow-you-full-control-and-flexibility-over-every-element-and-process-in-your-medias-life-cycle-
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
---