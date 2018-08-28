swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 1
info:
  title: AWS Auto Scaling API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=EnterStandby:
    get:
      summary: Enter Standby
      description: Moves the specified instances into Standby mode.
      operationId: enterStandby
      x-api-path-slug: actionenterstandby-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: InstanceIds.member.N
        description: One or more instances to move into Standby mode
        type: string
      - in: query
        name: ShouldDecrementDesiredCapacity
        description: Specifies whether the instances moved to Standby mode count as
          part of the Auto Scaling groups desired capacity
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stand By
  /?Action=ExitStandby:
    get:
      summary: Exit Standby
      description: Moves the specified instances out of Standby mode.
      operationId: exitStandby
      x-api-path-slug: actionexitstandby-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: InstanceIds.member.N
        description: One or more instance IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stand By