---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 1
info:
  title: SendGrid
  description: the-sendgrid-web-api-v3-documentation--this-is-the-entirety-of-the-documented-v3-endpoints--we-have-updated-all-the-descriptions-parameters-requests-and-responses--authentication-every-endpoint-requires-authentication-in-the-form-of-an-authorization-header-authorization-bearer-api-key
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /campaigns/{campaign_id}/schedules:
    delete:
      summary: Delete Campaigns Campaign  Schedules
      description: |-
        **This endpoint allows you to unschedule a campaign that has already been scheduled to be sent.**

        A successful unschedule will return a 204.
        If the specified campaign is in the process of being sent, the only option is to cancel (a different method).

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.schedules.delete
      x-api-path-slug: campaignscampaign-idschedules-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
      - ""
      - Schedules
    get:
      summary: Get Campaigns Campaign  Schedules
      description: |-
        **This endpoint allows you to retrieve the date and time that the given campaign has been scheduled to be sent.**

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.schedules.get
      x-api-path-slug: campaignscampaign-idschedules-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
      - ""
      - Schedules
    patch:
      summary: Patch Campaigns Campaign  Schedules
      description: |-
        **This endpoint allows to you change the scheduled time and date for a campaign to be sent.**

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.schedules.patch
      x-api-path-slug: campaignscampaign-idschedules-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
      - ""
      - Schedules
    post:
      summary: Add Campaigns Campaign  Schedules
      description: |-
        **This endpoint allows you to schedule a specific date and time for your campaign to be sent.**

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.schedules.post
      x-api-path-slug: campaignscampaign-idschedules-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
      - ""
      - Schedules
  /campaigns/{campaign_id}/schedules/now:
    post:
      summary: Add Campaigns Campaign  Schedules Now
      description: |-
        **This endpoint allows you to immediately send a campaign at the time you make the API call.**

        Normally a POST would have a request body, but since this endpoint is telling us to send a resource that is already created, a request body is not needed.

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.schedules.now.post
      x-api-path-slug: campaignscampaign-idschedulesnow-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
      - ""
      - Schedules
      - Now
  /campaigns/{campaign_id}/schedules/test:
    post:
      summary: Add Campaigns Campaign  Schedules Test
      description: |-
        **This endpoint allows you to send a test campaign.**

        To send to multiple addresses, use an array for the JSON "to" value ["one@address","two@address"]

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.schedules.test.post
      x-api-path-slug: campaignscampaign-idschedulestest-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
      - ""
      - Schedules
      - Test
---