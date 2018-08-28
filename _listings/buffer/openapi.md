swagger: "2.0"
x-collection-name: Buffer
x-complete: 1
info:
  title: Bufferapp
  description: social-media-management-for-marketers-and-agencies
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