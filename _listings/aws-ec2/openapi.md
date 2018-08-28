swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=MoveAddressToVpc:
    get:
      summary: Move Address To Vpc
      description: Moves an Elastic IP address from the EC2-Classic platform to the
        EC2-VPC platform.
      operationId: moveaddresstovpc
      x-api-path-slug: actionmoveaddresstovpc-get
      parameters:
      - in: query
        name: AllocationId
        description: '[EC2-VPC] The allocation ID'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: PublicIp
        description: '[EC2-Classic] The Elastic IP address'
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Address