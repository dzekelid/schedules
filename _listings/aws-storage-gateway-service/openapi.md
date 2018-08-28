swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 1
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteSnapshotSchedule:
    get:
      summary: Delete Snapshot Schedule
      description: Deletes a snapshot of a volume.
      operationId: deleteSnapshotSchedule
      x-api-path-slug: actiondeletesnapshotschedule-get
      parameters:
      - in: query
        name: VolumeARN
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DescribeSnapshotSchedule:
    get:
      summary: Describe Snapshot Schedule
      description: Describes the snapshot schedule for the specified gateway volume.
      operationId: describeSnapshotSchedule
      x-api-path-slug: actiondescribesnapshotschedule-get
      parameters:
      - in: query
        name: VolumeARN
        description: The Amazon Resource Name (ARN) of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=UpdateSnapshotSchedule:
    get:
      summary: Update Snapshot Schedule
      description: Updates a snapshot schedule configured for a gateway volume.
      operationId: updateSnapshotSchedule
      x-api-path-slug: actionupdatesnapshotschedule-get
      parameters:
      - in: query
        name: Description
        description: Optional description of the snapshot that overwrites the existing         description
        type: string
      - in: query
        name: RecurrenceInHours
        description: Frequency of snapshots
        type: string
      - in: query
        name: StartAt
        description: The hour of the day at which the snapshot schedule begins represented
          as            hh, where hh is the hour (0 to 23)
        type: string
      - in: query
        name: VolumeARN
        description: The Amazon Resource Name (ARN) of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots