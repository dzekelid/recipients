---
swagger: "2.0"
info:
  title: Dyn Activate Recipient(s)
  version: 1.0.0
  description: Activating a specified Recipientu2019s status
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
      - activate
      - recipients
definitions: []
x-collection-name: Dyn
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