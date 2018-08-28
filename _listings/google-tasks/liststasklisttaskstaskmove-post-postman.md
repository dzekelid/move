{
  "info": {
    "name": "Google Tasks API Add Lists Task List Tasks Task Move",
    "_postman_id": "a0ff63f2-5d07-4f50-9f29-9b349a377dae",
    "description": "Moves the specified task to another position in the task list. This can include putting it as a child task under a new parent and/or move it to a different position among its sibling tasks.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "lists",
      "item": [
        {
          "id": "835a100a-2e31-4c6d-99a0-3af442f10632",
          "name": "tasks.tasks.move",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "tasks",
                "v1",
                "lists/:tasklist/tasks/:task/move"
              ],
              "query": [
                {
                  "key": "parent",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "previous",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "task",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "tasklist",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Moves the specified task to another position in the task list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "774f8472-5a74-4f4f-a882-cc9c80231268"
            }
          ]
        }
      ]
    }
  ]
}