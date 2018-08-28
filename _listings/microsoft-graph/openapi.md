swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
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
  /users/{id | userPrincipalName}/messages/{id}/move:
    post:
      summary: Message Move
      description: 'message: move Move a message to a folder. This creates a new copy
        of the message in the destination folder.'
      operationId: Message:Move
      x-api-path-slug: usersid--userprincipalnamemessagesidmove-post
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
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Message
      - Move
  /me/mailFolders/{id}/messages/{id}/move:
    post:
      summary: Message Move
      description: 'message: move Move a message to a folder. This creates a new copy
        of the message in the destination folder.'
      operationId: Message:Move
      x-api-path-slug: memailfoldersidmessagesidmove-post
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
  /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move:
    post:
      summary: Message Move
      description: 'message: move Move a message to a folder. This creates a new copy
        of the message in the destination folder.'
      operationId: Message:Move
      x-api-path-slug: usersid--userprincipalnamemailfoldersidmessagesidmove-post
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
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Message
      - Move