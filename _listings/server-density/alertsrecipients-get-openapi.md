---
swagger: "2.0"
x-collection-name: Server Density
x-complete: 0
info:
  title: Alerts API Alerts Recipients
  description: Gets a list of all alert recipient's targets that are visible to you
    as a customer.
  version: 1.0.0
host: api.serverdensity.io.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  '/alerts/recipients ':
    ' get ':
      summary: Alerts Recipients
      description: Gets a list of all alert recipient's targets that are visible to
        you as a customer.
      operationId: -alerts-recipients-
      x-api-path-slug: alertsrecipients-get
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/recipients/{recipient_id} ':
    ' get ':
      summary: Alerts Recipients
      description: Gets a information about alert recipient's targets.
      operationId: -alerts-recipients-recipient-id-
      x-api-path-slug: alertsrecipientsrecipient-id-get
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/recipient ':
    ' post ':
      summary: Alerts Recipient
      description: Creates a new recipient with one sms and one email target associated.
      operationId: -alerts-recipient-
      x-api-path-slug: alertsrecipient-post
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/recipient/{recipient_id} ':
    ' put ':
      summary: Alerts Recipient
      description: Updates recipient along with sms and email targets associated.
      operationId: -alerts-recipient-recipient-id-
      x-api-path-slug: alertsrecipientrecipient-id-put
      responses:
        200:
          description: OK
      tags:
      - Alerts
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