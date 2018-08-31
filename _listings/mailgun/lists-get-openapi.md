---
swagger: "2.0"
x-collection-name: Mailgun
x-complete: 0
info:
  title: Mailgun API Lists
  description: Returns a list of mailing lists under your account.
  version: v2
host: api.mailgun.net
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  bounces/:
    get:
      summary: Bounces
      description: Fetches the list of bounces.
      operationId: getBounces
      x-api-path-slug: bounces-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of records to return
      - in: query
        name: skip
        description: Number of records to skip
      responses:
        200:
          description: OK
      tags:
      - Bounces
    post:
      summary: Add Bounce
      description: Adds a permanent bounce to the bounces table. Updates the existing
        record if already here.
      operationId: postBounces
      x-api-path-slug: bounces-post
      parameters:
      - in: query
        name: address
        description: Email address to add to bounce list
      - in: query
        name: code
        description: Error code (default 550)
      - in: query
        name: error
        description: Error description, (default is empty)
      responses:
        200:
          description: OK
      tags:
      - Bounce
  bounces/{address}:
    delete:
      summary: Delete Bounce
      description: Clears a bounce event.
      operationId: deleteBouncesAddress
      x-api-path-slug: bouncesaddress-delete
      responses:
        200:
          description: OK
      tags:
      - Bounce
    get:
      summary: Bounce
      description: Fetches a single bounce event by a given email address. This is
        useful to check if a given email address has bounced before.
      operationId: getBouncesAddress
      x-api-path-slug: bouncesaddress-get
      parameters:
      - in: path
        name: address
        description: The email address to get bounce request for
      responses:
        200:
          description: OK
      tags:
      - Bounce
  complaints/:
    get:
      summary: Complaints
      description: Fetches the list of complaints.
      operationId: getComplaints
      x-api-path-slug: complaints-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of records to return
      - in: query
        name: skip
        description: Number of records to skip
      responses:
        200:
          description: OK
      tags:
      - Complaints
    post:
      summary: Add Complaint
      description: Adds an address to the complaints table.
      operationId: postComplaints
      x-api-path-slug: complaints-post
      parameters:
      - in: query
        name: address
        description: Email address to add to the complaint list
      responses:
        200:
          description: OK
      tags:
      - Complaint
  complaints/{address}:
    delete:
      summary: Delete Complaint
      description: Removes a given spam complaint.
      operationId: deleteComplaintsAddress
      x-api-path-slug: complaintsaddress-delete
      parameters:
      - in: query
        name: address
        description: Email address of complaint to remove
      responses:
        200:
          description: OK
      tags:
      - Complaint
    get:
      summary: Complaint
      description: Fetches a single spam complaint by a given email address. This
        is useful to check if a particular user has complained.
      operationId: getComplaintsAddress
      x-api-path-slug: complaintsaddress-get
      parameters:
      - in: query
        name: address
        description: Email address of the complaint to get
      responses:
        200:
          description: OK
      tags:
      - Complaint
  lists:
    post:
      summary: Create List
      description: Creates a new mailing list.
      operationId: postLists
      x-api-path-slug: lists-post
      parameters:
      - in: query
        name: access_level
        description: 'List access level, one of: readonly (default), members, everyone'
      - in: query
        name: address
        description: A valid email address for the mailing list, e
      - in: query
        name: description
        description: A description
      - in: query
        name: name
        description: Mailing list name, e
      responses:
        200:
          description: OK
      tags:
      - List
  lists/:
    get:
      summary: Lists
      description: Returns a list of mailing lists under your account.
      operationId: getLists
      x-api-path-slug: lists-get
      parameters:
      - in: query
        name: access_level
        description: 'List access level, one of: readonly (default), members, everyone'
      - in: query
        name: address
        description: Find a mailing list by itu2019s address (optional)
      - in: query
        name: description
        description: Description string
      - in: query
        name: limit
        description: Maximum number of records to return (100 by default)
      - in: query
        name: namespace_id
        description: New name, e
      - in: query
        name: skip
        description: Records to skip (0 by default)
      responses:
        200:
          description: OK
      tags:
      - Lists
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