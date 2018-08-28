swagger: "2.0"
x-collection-name: Dropbox
x-complete: 1
info:
  title: Dropbox Notify Appendix API v1
  description: the-dropbox-notify--is-a-part-of-dropbox-core-ap-with-a-separate-endpoint-for-notification-call-
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api-notify.dropbox.com
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