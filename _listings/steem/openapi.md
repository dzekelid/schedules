swagger: "2.0"
x-collection-name: Steem
x-complete: 1
info:
  title: Interactive Steem API
  description: interactive-steem-api-lets-you-interact-with-steem-blockchain-and-make-a-request-get-output-and-start-implementing-new-apps-apis-have-default-parameters-set-to-get-you-started-and-see-how-request-works--api-list-is-compiled-from-steem-githubhttpsgithub-comsteemitsteem-1httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappapi-hpp-and-2httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappdatabase-api-hpp--if-you-want-to-contribute-documenting-detail-of-properties-and-output-contact-goodkarmahttpssteemit-chatdirectgoodkarma--you-can-also-check-full-list-here-steem-jshttpssteemjs-com
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_witness_schedule:
    get:
      summary: get_witness_schedule
      description: get_witness_schedule
      operationId: get-witness-schedule
      x-api-path-slug: get-witness-schedule-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Witness
      - Schedule
  /get_next_scheduled_hardfork:
    get:
      summary: get_next_scheduled_hardfork
      description: get_next_scheduled_hardfork
      operationId: get-next-scheduled-hardfork
      x-api-path-slug: get-next-scheduled-hardfork-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Next
      - Scheduled
      - Hardfork