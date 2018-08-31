---
name: Mailgun
x-slug: mailgun
description: Mailgun provides a web service for integrating email inboxes into apps.
  Providing APIs for sending, receiving, and storing APis, including tools for managing
  delivery, real-time integration, organizing, routing, and tracking on emails. Malign
  provides a free trial to learn about services, and pay as you go, unit based pricing
  to continue from there, including volume pricing for increased usage.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
x-kinRank: "8"
x-alexaRank: "24750"
tags: Mailgun
created: "2018-08-30"
modified: "2018-08-30"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/apis.md
specificationVersion: "0.14"
apis:
- name: Mailgun API - Bounces
  x-api-slug: bounces-get
  description: Fetches the list of bounces.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/bounces-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/bounces-get-openapi.md
- name: Mailgun API - Add Bounce
  x-api-slug: bounces-post
  description: Adds a permanent bounce to the bounces table. Updates the existing
    record if already here.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/bounces-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/bounces-post-openapi.md
- name: Mailgun API - Delete Bounce
  x-api-slug: bouncesaddress-delete
  description: Clears a bounce event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/bouncesaddress-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/bouncesaddress-delete-openapi.md
- name: Mailgun API - Bounce
  x-api-slug: bouncesaddress-get
  description: Fetches a single bounce event by a given email address. This is useful
    to check if a given email address has bounced before.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/bouncesaddress-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/bouncesaddress-get-openapi.md
- name: Mailgun API - Complaints
  x-api-slug: complaints-get
  description: Fetches the list of complaints.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/complaints-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/complaints-get-openapi.md
- name: Mailgun API - Add Complaint
  x-api-slug: complaints-post
  description: Adds an address to the complaints table.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/complaints-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/complaints-post-openapi.md
- name: Mailgun API - Delete Complaint
  x-api-slug: complaintsaddress-delete
  description: Removes a given spam complaint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/complaintsaddress-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/complaintsaddress-delete-openapi.md
- name: Mailgun API - Complaint
  x-api-slug: complaintsaddress-get
  description: Fetches a single spam complaint by a given email address. This is useful
    to check if a particular user has complained.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/complaintsaddress-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/complaintsaddress-get-openapi.md
- name: Mailgun API - Create List
  x-api-slug: lists-post
  description: Creates a new mailing list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/lists-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/lists-post-openapi.md
- name: Mailgun API - Lists
  x-api-slug: lists-get
  description: Returns a list of mailing lists under your account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/lists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/lists-get-openapi.md
- name: Mailgun API - Delete List
  x-api-slug: listsaddress-delete
  description: Deletes a mailing list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/listsaddress-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/listsaddress-delete-openapi.md
- name: Mailgun API - List
  x-api-slug: listsaddress-get
  description: Returns a single mailing list by a given address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/listsaddress-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/listsaddress-get-openapi.md
- name: Mailgun API - Update List
  x-api-slug: listsaddress-put
  description: Update mailing list properties, such as address, description or name
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/listsaddress-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/listsaddress-put-openapi.md
- name: Mailgun API - Add To List
  x-api-slug: listsaddressmembers-get
  description: Adds a member to the mailing list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/listsaddressmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/listsaddressmembers-get-openapi.md
- name: Mailgun API - List Members
  x-api-slug: listsaddressmembers-get
  description: Fetches the list of mailing list members.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/listsaddressmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/listsaddressmembers-get-openapi.md
- name: Mailgun API - List Member
  x-api-slug: listsaddressmembersmember-address-get
  description: Retrieves a mailing list member.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/listsaddressmembersmember-address-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/listsaddressmembersmember-address-get-openapi.md
- name: Mailgun API - Posts Mime Message
  x-api-slug: messages-mime-post
  description: 'Posts a message in MIME format. Note: you will need to build a MIME
    string yourself. Use a MIME library for your programming language to do this.
    Pass the resulting MIME string as message parameter.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/messages-mime-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/messages-mime-post-openapi.md
- name: Mailgun API - Send Message
  x-api-slug: messages-post
  description: Sends a message by assembling it from the components. Note that you
    can specify most parameters multiple times, HTTP supports this out of the box.
    This makes sense for parameters like cc, to or attachment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/messages-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/messages-post-openapi.md
- name: Mailgun API - Message
  x-api-slug: messagesid-get
  description: Gets a message.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/messagesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/messagesid-get-openapi.md
- name: Mailgun API - Routes
  x-api-slug: routes-get
  description: Fetches the list of routes. Note that routes are defined globally,
    per account, not per domain as most of other API calls.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/routes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/routes-get-openapi.md
- name: Mailgun API - Add Route
  x-api-slug: routes-post
  description: Creates a new route.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/routes-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/routes-post-openapi.md
- name: Mailgun API - Delete Route
  x-api-slug: routesid-delete
  description: Deletes a route based on the id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/routesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/routesid-delete-openapi.md
- name: Mailgun API - Route
  x-api-slug: routesid-get
  description: Returns a single route object based on its ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/routesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/routesid-get-openapi.md
- name: Mailgun API - Updates Route
  x-api-slug: routesid-put
  description: Updates a given route by ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/routesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/routesid-put-openapi.md
- name: Mailgun API - Stats
  x-api-slug: stats-get
  description: Returns a list of event stat items. Each record represents counts for
    one event per one day.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/stats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/stats-get-openapi.md
- name: Mailgun API - Delete Tag
  x-api-slug: tagstag-delete
  description: Deletes all counters for particular tag and the tag itself.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/tagstag-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/tagstag-delete-openapi.md
- name: Mailgun API - Unsubscribes
  x-api-slug: unsubscribes-get
  description: This API allows you to programmatically download the list of recipients
    who have unsubscribed from your emails.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/unsubscribes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/unsubscribes-get-openapi.md
- name: Mailgun API - Add to unsubscribe list.
  x-api-slug: unsubscribes-post
  description: Adds address to unsubscribed table.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/unsubscribes-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/unsubscribes-post-openapi.md
- name: Mailgun API - Delete Unsubscribe
  x-api-slug: unsubscribesaddress-delete
  description: Removes an address from the unsubscribes table. Address defines which
    events to delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/unsubscribesaddress-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/unsubscribesaddress-delete-openapi.md
- name: Mailgun API - Unsubscribe
  x-api-slug: unsubscribesaddress-get
  description: Retreives a single unsubscribe record. Can be used to check if a given
    address is present in the list of unsubscribed users.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/unsubscribesaddress-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/mailgun/master/_listings/mailgun/unsubscribesaddress-get-openapi.md
x-common:
- type: x--net-library
  url: http://documentation.mailgun.com/libraries.html#c
- type: x-api-gallery
  url: http://lykke.api.gallery.streamdata.io
- type: x-api-stack
  url: http://mailgun.stack.network
- type: x-base
  url: https://api.mailgun.net
- type: x-blog
  url: http://blog.mailgun.net
- type: x-blog-rss
  url: https://twitter.com/unbounce
- type: x-crunchbase
  url: http://www.crunchbase.com/company/mailgun
- type: x-crunchbase
  url: https://crunchbase.com/organization/mailgun
- type: x-developer
  url: http://documentation.mailgun.com/
- type: x-email
  url: privacy@mailgun.com
- type: x-faq
  url: http://documentation.mailgun.com/faqs.html
- type: x-github
  url: https://github.com/mailgun
- type: x-heroku-addon
  url: https://addons.heroku.com/mailgun
- type: x-java-library
  url: http://documentation.mailgun.com/libraries.html#java
- type: x-node-js-library
  url: http://documentation.mailgun.com/libraries.html#node-js
- type: x-php-library
  url: http://documentation.mailgun.com/libraries.html#php
- type: x-pricing
  url: http://www.mailgun.com/pricing
- type: x-privacy
  url: http://www.mailgun.com/privacy
- type: x-python-library
  url: http://documentation.mailgun.com/libraries.html#python
- type: x-ruby-library
  url: http://documentation.mailgun.com/libraries.html#ruby
- type: x-selfservice-registration
  url: https://www.mailgun.com/signup
- type: x-stack-overflow
  url: https://stackoverflow.com/questions/tagged/mailgun
- type: x-terms-of-service
  url: http://www.mailgun.com/terms
- type: x-twitter
  url: https://twitter.com/#!/mail_gun
- type: x-website
  url: http://mailgun.net
- type: x-wordpress-plugin
  url: https://wordpress.org/plugins/mailgun/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---