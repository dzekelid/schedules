---
name: SendGrid
x-slug: sendgrid
description: Delivering your transactional and marketing emails through the worlds
  largest cloud-based email delivery platform. Send with confidence.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
x-kinRank: "9"
x-alexaRank: "9582"
tags: Schedules
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/sendgrid/apis.md
specificationVersion: "0.14"
apis:
- name: SendGrid Delete Campaigns Campaign  Schedules
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to unschedule a campaign that has already been scheduled to be sent.**

    A successful unschedule will return a 204.
    If the specified campaign is in the process of being sent, the only option is to cancel (a different method).

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns/{campaign_id}/schedules
  tags: Email,Campaigns, Campaign, , Schedules
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/sendgrid/campaignscampaign-idschedules-delete-openapi.md
- name: SendGrid Get Campaigns Campaign  Schedules
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the date and time that the given campaign has been scheduled to be sent.**

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns/{campaign_id}/schedules
  tags: Email,Campaigns, Campaign, , Schedules
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/sendgrid/campaignscampaign-idschedules-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/sendgrid/campaignscampaign-idschedules-get-openapi.md
- name: SendGrid Patch Campaigns Campaign  Schedules
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows to you change the scheduled time and date for a campaign to be sent.**

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns/{campaign_id}/schedules
  tags: Email,Campaigns, Campaign, , Schedules
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/sendgrid/campaignscampaign-idschedules-patch-openapi.md
- name: SendGrid Add Campaigns Campaign  Schedules
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to schedule a specific date and time for your campaign to be sent.**

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns/{campaign_id}/schedules
  tags: Email,Campaigns, Campaign, , Schedules
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/sendgrid/campaignscampaign-idschedules-post-openapi.md
- name: SendGrid Add Campaigns Campaign  Schedules Now
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to immediately send a campaign at the time you make the API call.**

    Normally a POST would have a request body, but since this endpoint is telling us to send a resource that is already created, a request body is not needed.

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns/{campaign_id}/schedules/now
  tags: Email,Campaigns, Campaign, , Schedules, Now
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/sendgrid/campaignscampaign-idschedulesnow-post-openapi.md
- name: SendGrid Add Campaigns Campaign  Schedules Test
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to send a test campaign.**

    To send to multiple addresses, use an array for the JSON "to" value ["one@address","two@address"]

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns/{campaign_id}/schedules/test
  tags: Email,Campaigns, Campaign, , Schedules, Test
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/sendgrid/campaignscampaign-idschedulestest-post-openapi.md
- name: SendGrid
  x-api-slug: sendgrid
  description: SendGrids cloud-based email infrastructure relieves businesses of the
    cost and complexity of maintaining custom email systems. SendGrid provides reliable
    delivery, scalability and real-time analytics along with flexible APIs that make
    custom integration a breeze.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: Schedules
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/sendgrid/openapi.md
x-common:
- type: x--net-library
  url: https://sendgrid.com/docs/Code_Examples/csharp.html
- type: x-base
  url: https://api.sendgrid.com
- type: x-blog
  url: http://blog.sendgrid.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/sendgrid/CDXr
- type: x-contact-form
  url: https://sendgrid.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/sendgrid
- type: x-crunchbase
  url: https://crunchbase.com/organization/sendgrid
- type: x-developer
  url: https://sendgrid.com/developers
- type: x-documentation
  url: https://sendgrid.com/docs/index.html
- type: x-email
  url: privacy@sendgrid.com
- type: x-email
  url: legal@sendgrid.com
- type: x-email
  url: dpo@sendgrid.com
- type: x-forum
  url: http://support.sendgrid.com/forums
- type: x-github
  url: https://github.com/sendgrid
- type: x-go-library
  url: https://sendgrid.com/docs/Code_Examples/go.html
- type: x-ios-library
  url: https://sendgrid.com/docs/Code_Examples/ios.html
- type: x-java-library
  url: https://sendgrid.com/docs/Code_Examples/java.html
- type: x-labs
  url: http://labs.sendgrid.com/
- type: x-node-js-library
  url: https://sendgrid.com/docs/Code_Examples/nodejs.html
- type: x-partners
  url: https://sendgrid.com/partners
- type: x-perl-library
  url: https://sendgrid.com/docs/Code_Examples/perl.html
- type: x-php-library
  url: https://sendgrid.com/docs/Code_Examples/php.html
- type: x-pricing
  url: https://sendgrid.com/transactional-email/pricing
- type: x-privacy
  url: https://sendgrid.com/privacy
- type: x-python-library
  url: https://sendgrid.com/docs/Code_Examples/python.html
- type: x-ruby-library
  url: https://sendgrid.com/docs/Code_Examples/ruby.html
- type: x-security
  url: https://sendgrid.com/security
- type: x-selfservice-registration
  url: https://sendgrid.com/user/signup
- type: x-terms-of-service
  url: https://sendgrid.com/tos
- type: x-twitter
  url: https://twitter.com/SendGrid
- type: x-website
  url: http://sendgrid.com
- type: x-website
  url: https://sendgrid.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---