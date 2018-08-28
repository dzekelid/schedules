---
name: Urban Airship
x-slug: urban-airship
description: A market-leading mobile app engagement, mobile analytics, mobile data
  integration and mobile wallet marketing solution.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
x-kinRank: "8"
x-alexaRank: "79571"
tags: Schedules
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/apis.md
specificationVersion: "0.14"
apis:
- name: Urban Airship - Delete Push Scheduled Notification
  x-api-slug: pushschedulednotification-delete
  description: Cancels a scheduled notification.  A successful delete will have an
    HTTP status code of 204. If the scheduled notification does not exist, has already
    been successfully deleted, or was sent, the status code will be 404.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushschedulednotification-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushschedulednotification-delete-openapi.md
- name: Urban Airship - Post Push Scheduled
  x-api-slug: pushscheduled-post
  description: Bulk deletes scheduled notifications. If you include URLs or aliases
    for scheduled notifications that don???t exist or have already been sent, they
    will be ignored. Any device token in the cancel_device_tokens payload will have
    every notification that is sent to it removed. This will not prevent it from receiving
    scheduled notifications to tags or broadcast messages.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduled-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduled-post-openapi.md
- name: Urban Airship - Put Push Scheduled Alias Alias
  x-api-slug: pushscheduledaliasalias-put
  description: Changes a scheduled notification alias. Aliases for scheduled notifications
    are unique per Urban Airship application, so you might want to hash the aliases
    with a device ID or use some other mechanism to ensure uniqueness. The only other
    limit is that they must be 255 characters or less.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduledaliasalias-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduledaliasalias-put-openapi.md
- name: Urban Airship - Delete Push Scheduled Alias Alias
  x-api-slug: pushscheduledaliasalias-delete
  description: Deletes a scheduled notification alias.  If you attempt to schedule
    an aliased scheduled notification with an alias that already exists for your application,
    it will overwrite the existing one.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduledaliasalias-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduledaliasalias-delete-openapi.md
- name: Urban Airship - Delete Push Scheduled Notification
  x-api-slug: pushschedulednotification-delete
  description: Cancels a scheduled notification.  A successful delete will have an
    HTTP status code of 204. If the scheduled notification does not exist, has already
    been successfully deleted, or was sent, the status code will be 404.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushschedulednotification-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushschedulednotification-delete-openapi.md
- name: Urban Airship - Post Push Scheduled
  x-api-slug: pushscheduled-post
  description: Bulk deletes scheduled notifications. If you include URLs or aliases
    for scheduled notifications that don???t exist or have already been sent, they
    will be ignored. Any device token in the cancel_device_tokens payload will have
    every notification that is sent to it removed. This will not prevent it from receiving
    scheduled notifications to tags or broadcast messages.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduled-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduled-post-openapi.md
- name: Urban Airship - Put Push Scheduled Alias Alias
  x-api-slug: pushscheduledaliasalias-put
  description: Changes a scheduled notification alias. Aliases for scheduled notifications
    are unique per Urban Airship application, so you might want to hash the aliases
    with a device ID or use some other mechanism to ensure uniqueness. The only other
    limit is that they must be 255 characters or less.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduledaliasalias-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduledaliasalias-put-openapi.md
- name: Urban Airship - Delete Push Scheduled Alias Alias
  x-api-slug: pushscheduledaliasalias-delete
  description: Deletes a scheduled notification alias.  If you attempt to schedule
    an aliased scheduled notification with an alias that already exists for your application,
    it will overwrite the existing one.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduledaliasalias-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduledaliasalias-delete-openapi.md
- name: Urban Airship - Delete Push Scheduled Alias Alias
  x-api-slug: pushscheduledaliasalias-delete
  description: Deletes a scheduled notification alias.  If you attempt to schedule
    an aliased scheduled notification with an alias that already exists for your application,
    it will overwrite the existing one.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduledaliasalias-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduledaliasalias-delete-openapi.md
- name: Urban Airship - Put Push Scheduled Alias Alias
  x-api-slug: pushscheduledaliasalias-put
  description: Changes a scheduled notification alias. Aliases for scheduled notifications
    are unique per Urban Airship application, so you might want to hash the aliases
    with a device ID or use some other mechanism to ensure uniqueness. The only other
    limit is that they must be 255 characters or less.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduledaliasalias-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduledaliasalias-put-openapi.md
- name: Urban Airship - Post Push Scheduled
  x-api-slug: pushscheduled-post
  description: Bulk deletes scheduled notifications. If you include URLs or aliases
    for scheduled notifications that don???t exist or have already been sent, they
    will be ignored. Any device token in the cancel_device_tokens payload will have
    every notification that is sent to it removed. This will not prevent it from receiving
    scheduled notifications to tags or broadcast messages.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduled-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushscheduled-post-openapi.md
- name: Urban Airship - Delete Push Scheduled Notification
  x-api-slug: pushschedulednotification-delete
  description: Cancels a scheduled notification.  A successful delete will have an
    HTTP status code of 204. If the scheduled notification does not exist, has already
    been successfully deleted, or was sent, the status code will be 404.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushschedulednotification-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/schedules/master/_listings/urban-airship/pushschedulednotification-delete-openapi.md
x-common:
- type: x-website
  url: http://urbanairship.com/
- type: x-android-sdk
  url: http://docs.urbanairship.com/platform/android.html
- type: x-api-gallery
  url: http://ulster.bank.api.gallery.streamdata.io
- type: x-api-stack
  url: http://urban.airship.stack.network
- type: x-blackberry-sdk
  url: http://docs.urbanairship.com/platform/blackberry.html
- type: x-blog
  url: http://urbanairship.com/blog
- type: x-blog-rss
  url: http://urbanairship.com/blog/rss
- type: x-case-studies
  url: http://urbanairship.com/resources/case-studies
- type: x-crunchbase
  url: http://www.crunchbase.com/company/urban-airship
- type: x-crunchbase
  url: https://crunchbase.com/organization/urban-airship
- type: x-developer
  url: http://docs.urbanairship.com/
- type: x-email
  url: legal@urbanairship.com
- type: x-email
  url: privacy@urbanairship.com
- type: x-email
  url: support@urbanairship.com
- type: x-github
  url: https://github.com/urbanairship
- type: x-glossary
  url: http://docs.urbanairship.com/reference/glossary.html
- type: x-ios-sdk
  url: http://docs.urbanairship.com/platform/ios.html
- type: x-linkedin
  url: https://www.linkedin.com/company/urban-airship/
- type: x-phonegap-sdk
  url: http://docs.urbanairship.com/platform/phonegap.html
- type: x-pricing
  url: https://www.urbanairship.com/products/engage/pricing
- type: x-privacy
  url: http://urbanairship.com/legal/privacy-policy
- type: x-security
  url: http://docs.urbanairship.com/reference/app_keys_secrets.html
- type: x-twitter
  url: https://twitter.com/urbanairship
- type: x-website
  url: http://urbanairship.com
- type: x-white-papers
  url: http://urbanairship.com/resources/whitepapers
- type: x-windows-sdk
  url: http://docs.urbanairship.com/platform/windows.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---