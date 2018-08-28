---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Delete a scheduled custom event
  description: Delete a scheduled custom event with predefined identifier string
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /queue/payments:
    get:
      summary: Retrieve a scheduled payment list
      description: Retrieve a scheduled payment list
      operationId: queue.payments.get
      x-api-path-slug: queuepayments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Scheduled
      - Payment
      - List
  /queue/payments/{id}:
    get:
      summary: Retrieve a scheduled payment
      description: Retrieve a payment with specified identifier string
      operationId: queue.payments.id.get
      x-api-path-slug: queuepaymentsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Scheduled
      - Payment
  /queue/custom-events:
    get:
      summary: Retrieve a list of scheduled custom events
      description: Retrieve a list of scheduled custom events
      operationId: retrieve-a-list-of-scheduled-custom-events
      x-api-path-slug: queuecustomevents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Scheduled
      - Custom
      - Events
  /queue/custom-events/{id}:
    delete:
      summary: Delete a scheduled custom event
      description: Delete a scheduled custom event with predefined identifier string
      operationId: delete-a-scheduled-custom-event-with-predefined-identifier-string
      x-api-path-slug: queuecustomeventsid-delete
      responses:
        200:
          description: OK
      tags:
      - Scheduled
      - Custom
      - Event
    get:
      summary: Retrieve a scheduled custom event
      description: Retrieve a scheduled custom event with predefined identifier string
      operationId: retrieve-a-scheduled-custom-event-with-predefined-identifier-string
      x-api-path-slug: queuecustomeventsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Scheduled
      - Custom
      - Event
  /queue/payments/{id}/cancel:
    post:
      summary: Cancel a scheduled payment
      description: Cancel a scheduled payment with specified identifier string
      operationId: cancel-a-scheduled-payment-with-specified-identifier-string
      x-api-path-slug: queuepaymentsidcancel-post
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Scheduled
      - Payment
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