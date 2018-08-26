---
swagger: "2.0"
x-collection-name: Buffer
x-complete: 0
info:
  title: Buffer Post Updates Move To Top Mediatypeextension
  description: Move an existing status update to the top of the queue and recalculate
    times for all updates in the queue. Returns the update with its new posting time.
  version: "1"
host: api.bufferapp.com
basePath: /1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /updates/{id}/move_to_top{mediaTypeExtension}:
    post:
      summary: Post Updates Move To Top Mediatypeextension
      description: Move an existing status update to the top of the queue and recalculate
        times for all updates in the queue. Returns the update with its new posting
        time.
      operationId: move-an-existing-status-update-to-the-top-of-the-queue-and-recalculate-times-for-all-updates-in-the-
      x-api-path-slug: updatesidmove-to-topmediatypeextension-post
      parameters:
      - in: path
        name: id
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - Updates
      - Id
      - Move
      - To
      - TopmediaTypeExtension
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