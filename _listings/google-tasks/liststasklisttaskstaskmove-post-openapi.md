---
swagger: "2.0"
x-collection-name: Google Tasks
x-complete: 0
info:
  title: Google Tasks API Add Lists Task List Tasks Task Move
  description: Moves the specified task to another position in the task list. This
    can include putting it as a child task under a new parent and/or move it to a
    different position among its sibling tasks.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tasks/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lists/{tasklist}/tasks/{task}/move:
    post:
      summary: Add Lists Task List Tasks Task Move
      description: Moves the specified task to another position in the task list.
        This can include putting it as a child task under a new parent and/or move
        it to a different position among its sibling tasks.
      operationId: tasks.tasks.move
      x-api-path-slug: liststasklisttaskstaskmove-post
      parameters:
      - in: query
        name: parent
        description: New parent task identifier
      - in: query
        name: previous
        description: New previous sibling task identifier
      - in: path
        name: task
        description: Task identifier
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Task
      - List
      - Tasks
      - Task
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