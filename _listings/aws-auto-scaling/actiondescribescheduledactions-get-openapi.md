---
swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 0
info:
  title: AWS Auto Scaling API Describe Scheduled Actions
  version: 1.0.0
  description: Describes the actions scheduled for your Auto Scaling group that haven't
    run.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteScheduledAction:
    get:
      summary: Delete Scheduled Action
      description: Deletes the specified scheduled action.
      operationId: deleteScheduledAction
      x-api-path-slug: actiondeletescheduledaction-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: ScheduledActionName
        description: The name of the action to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scheduled Action
  /?Action=DescribeScheduledActions:
    get:
      summary: Describe Scheduled Actions
      description: Describes the actions scheduled for your Auto Scaling group that
        haven't run.
      operationId: describeScheduledActions
      x-api-path-slug: actiondescribescheduledactions-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: EndTime
        description: The latest scheduled start time to return
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: ScheduledActionNames.member.N
        description: Describes one or more scheduled actions
        type: string
      - in: query
        name: StartTime
        description: The earliest scheduled start time to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scheduled Actions
  /?Action=PutScheduledUpdateGroupAction:
    get:
      summary: Put Scheduled Update Group Action
      description: Creates or updates a scheduled scaling action for an Auto Scaling
        group.
      operationId: putScheduledUpdateGroupAction
      x-api-path-slug: actionputscheduledupdategroupaction-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name or Amazon Resource Name (ARN) of the Auto Scaling group
        type: string
      - in: query
        name: DesiredCapacity
        description: The number of EC2 instances that should be running in the group
        type: string
      - in: query
        name: EndTime
        description: The time for the recurring schedule to end
        type: string
      - in: query
        name: MaxSize
        description: The maximum size for the Auto Scaling group
        type: string
      - in: query
        name: MinSize
        description: The minimum size for the Auto Scaling group
        type: string
      - in: query
        name: Recurrence
        description: The recurring schedule for this action, in Unix cron syntax format
        type: string
      - in: query
        name: ScheduledActionName
        description: The name of this scaling action
        type: string
      - in: query
        name: StartTime
        description: The time for this action to start, in YYYY-MM-DDThh:mm:ssZ format
          in UTC/GMT only             (for example, 2014-06-01T00:00:00Z)
        type: string
      - in: query
        name: Time
        description: This parameter is deprecated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scheduled Update
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