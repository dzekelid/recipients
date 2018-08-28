swagger: "2.0"
x-collection-name: Dyn
x-complete: 1
info:
  title: Dyn
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  recipients/activate:
    post:
      summary: Activate Recipient(s)
      description: Activating a specified Recipientu2019s status
      operationId: postRecipientsActivate
      x-api-path-slug: recipientsactivate-post
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Recipients
  recipients/status:
    get:
      summary: Retrieve Recipient(s) Status
      description: Retrieve Recipient(s) Status
      operationId: getRecipientsStatus
      x-api-path-slug: recipientsstatus-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Recipients
      - Status