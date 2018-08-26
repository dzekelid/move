---
swagger: "2.0"
x-collection-name: Microsoft Office 365
x-complete: 1
info:
  title: Microsoft Office 365
  description: office-365-is-the-brand-name-used-by-microsoft-for-a-group-of-software-plus-services-subscriptions-that-provides-productivity-software-and-related-services-to-its-subscribers-
  version: 1.0.0
host: outlook.office365.com
basePath: /ews/odata/Me
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Messages{message_id}/Move:
    post:
      summary: Add Messages Message Move
      description: Post messages message  move
      operationId: postMessagesMessageMove
      x-api-path-slug: messagesmessage-idmove-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Move
    parameters:
      summary: Parameters Messages Message Move
      description: Parameters messages message  move
      operationId: parametersMessagesMessageMove
      x-api-path-slug: messagesmessage-idmove-parameters
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Move
---