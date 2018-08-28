swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/scheduler/jobs:
    post:
      summary: Create a scheduler job.
      description: Creates the scheduler job with a generated id. Set the state value
        to 'Active' to start the job. Set the state value to 'Inactive' to avoid starting
        the job.
      operationId: createJob
      x-api-path-slug: apiv1schedulerjobs-post
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: header
        name: Refresh-Token-For-Job-Execution
        description: Refresh-Token-For-Job-Execution
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Scheduler
      - Job
  /api/v1/scheduler/jobs/{id}:
    get:
      summary: Get a scheduler job by id.
      description: Returns the scheduler job with the given id.
      operationId: retrieveJob
      x-api-path-slug: apiv1schedulerjobsid-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: Job id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Scheduler
      - Job
      - By
      - Id
    put:
      summary: Update an existing scheduler job.
      description: Updates the scheduled job. The updated changes will be effective
        from the next scheduling of this job. To suspend a job, update the job with
        state value 'Inactive'. To resume a job, update the job with state value 'Active'.
      operationId: updateJob
      x-api-path-slug: apiv1schedulerjobsid-put
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: header
        name: Refresh-Token-For-Job-Execution
        description: Refresh-Token-For-Job-Execution
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Existing
      - Scheduler
      - Job