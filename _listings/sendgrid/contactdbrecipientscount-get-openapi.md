---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Contactdb Recipients Count
  description: |-
    **This endpoint allows you to retrieve the total number of Marketing Campaigns recipients.**

    The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
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
    post:
      summary: Add Contactdb Lists List  Recipients
      description: |-
        **This endpoint allows you to add multiple recipients to a list.**

        Adds existing recipients to a list, passing in the recipient IDs to add. Recipient IDs should be passed exactly as they are returned from recipient endpoints.

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.list_id.recipients.post
      x-api-path-slug: contactdblistslist-idrecipients-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
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
  /contactdb/lists/{list_id}/recipients/{recipient_id}:
    delete:
      summary: Delete Contactdb Lists List  Recipients Recipient
      description: |-
        **This endpoint allows you to delete a single recipient from a list.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.list_id.recipients.recipient_id.delete
      x-api-path-slug: contactdblistslist-idrecipientsrecipient-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: list_id
        description: The ID of the list you are taking this recipient away from
      - in: query
        name: No Name
      - in: query
        name: recipient_id
        description: The ID of the recipient to take off the list
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
      - Recipient
    post:
      summary: Add Contactdb Lists List  Recipients Recipient
      description: |-
        **This endpoint allows you to add a single recipient to a list.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.list_id.recipients.recipient_id.post
      x-api-path-slug: contactdblistslist-idrecipientsrecipient-id-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
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
      - Recipient
  /contactdb/recipients:
    delete:
      summary: Delete Contactdb Recipients
      description: |-
        **This endpoint allows you to deletes one or more recipients.**

        The body of an API call to this endpoint must include an array of recipient IDs of the recipients you want to delete.

        The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
      operationId: contactdb.recipients.delete
      x-api-path-slug: contactdbrecipients-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Recipients
    get:
      summary: Get Contactdb Recipients
      description: |-
        **This endpoint allows you to retrieve all of your Marketing Campaigns recipients.**

        Batch deletion of a page makes it possible to receive an empty page of recipients before reaching the end of
        the list of recipients. To avoid this issue; iterate over pages until a 404 is retrieved.

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.recipients.get
      x-api-path-slug: contactdbrecipients-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: page
        description: Page index of first recipients to return (must be a positive
          integer)
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
      - Recipients
    patch:
      summary: Patch Contactdb Recipients
      description: |-
        **This endpoint allows you to update one or more recipients.**

        The body of an API call to this endpoint must include an array of one or more recipient objects.

        It is of note that you can add custom field data as parameters on recipient objects. We have provided an example using some of the default custom fields SendGrid provides.

        The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
      operationId: contactdb.recipients.patch
      x-api-path-slug: contactdbrecipients-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Recipients
    post:
      summary: Add Contactdb Recipients
      description: |-
        **This endpoint allows you to add a Marketing Campaigns recipient.**

        You can add custom field data as a parameter on this endpoint. We have provided an example using some of the default custom fields SendGrid provides.

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.recipients.post
      x-api-path-slug: contactdbrecipients-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Recipients
  /contactdb/recipients/billable_count:
    get:
      summary: Get Contactdb Recipients Billable Count
      description: |-
        **This endpoint allows you to retrieve the number of Marketing Campaigns recipients that you will be billed for.**

        You are billed for marketing campaigns based on the highest number of recipients you have had in your account at one time. This endpoint will allow you to know the current billable count value.

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.recipients.billable_count.get
      x-api-path-slug: contactdbrecipientsbillable-count-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Recipients
      - Billable
      - Count
  /contactdb/recipients/count:
    get:
      summary: Get Contactdb Recipients Count
      description: |-
        **This endpoint allows you to retrieve the total number of Marketing Campaigns recipients.**

        The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
      operationId: contactdb.recipients.count.get
      x-api-path-slug: contactdbrecipientscount-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Recipients
      - Count
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