---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Message Move
  description: 'message: move Move a message to a folder. This creates a new copy
    of the message in the destination folder.'
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/mailFolders/{id}/move:
    post:
      summary: Mail Folder Move
      description: 'mailFolder: move Move a mailfolder and its contents to another
        mailfolder.'
      operationId: MailFolder:Move
      x-api-path-slug: memailfoldersidmove-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mail
      - Folder
      - Move
  /users/{id | userPrincipalName}/mailFolders/{id}/move:
    post:
      summary: Mail Folder Move
      description: 'mailFolder: move Move a mailfolder and its contents to another
        mailfolder.'
      operationId: MailFolder:Move
      x-api-path-slug: usersid--userprincipalnamemailfoldersidmove-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mail
      - Folder
      - Move
  /me/messages/{id}/move:
    post:
      summary: Message Move
      description: 'message: move Move a message to a folder. This creates a new copy
        of the message in the destination folder.'
      operationId: Message:Move
      x-api-path-slug: memessagesidmove-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Message
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