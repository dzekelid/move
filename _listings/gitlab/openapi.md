swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/issues/{issue_id}/move:
    post:
      summary: Post Projects Issues Issue Move
      description: Post projects issues issue move.
      operationId: postV3ProjectsIdIssuesIssueIdMove
      x-api-path-slug: v3projectsidissuesissue-idmove-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: issue_id
        description: The ID of a project issue
      - in: formData
        name: to_project_id
        description: The ID of the new project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Move