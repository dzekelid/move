---
swagger: "2.0"
x-collection-name: Google Tasks
x-complete: 1
info:
  title: Tasks
  description: lets-you-manage-your-tasks-and-task-lists-
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
---