---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Contactdb Lists List  Recipients
  description: "**This endpoint allows you to retrieve all recipients on the list
    with the given ID.** \n\nThe Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
    recipients."
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
  /contactdb/lists/{list_id}/recipients:
    get:
      summary: Get Contactdb Lists List  Recipients
      description: "**This endpoint allows you to retrieve all recipients on the list
        with the given ID.** \n\nThe Contacts API helps you manage your [Marketing
        Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
        recipients."
      operationId: contactdb.lists.list_id.recipients.get
      x-api-path-slug: contactdblistslist-idrecipients-get
      parameters:
      - in: query
        name: list_id
        description: The ID of the list whose recipients you are requesting
      - in: query
        name: No Name
      - in: query
        name: page
        description: Page index of first recipient to return (must be a positive integer)
      - in: query
        name: page_size
        description: Number of recipients to return at a time (must be a positive
          integer between 1 and 1000)
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
      - List
      - ""
      - Recipients
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