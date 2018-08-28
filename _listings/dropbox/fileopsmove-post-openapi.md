---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 0
info:
  title: Dropbox Core Moves a file or folder to a new location.
  description: Moves a file or folder to a new location.
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api.dropbox.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /fileops/move:
    post:
      summary: Moves a file or folder to a new location.
      description: Moves a file or folder to a new location.
      operationId: moves-a-file-or-folder-to-a-new-location
      x-api-path-slug: fileopsmove-post
      parameters:
      - in: formData
        name: from_path
        description: Specifies the file or folder to be moved from relative to `root`
      - in: formData
        name: locale
        description: The metadata returned will have its `size` field translated based
          on the given locale
      - in: formData
        name: root
        description: The root relative to which `from_path` and `to_path` are specified
      - in: formData
        name: to_path
        description: Specifies the destination path, *including the new name for the
          file or folder*, relative to `root`
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Fileops
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