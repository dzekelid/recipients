swagger: "2.0"
x-collection-name: Server Density
x-complete: 1
info:
  title: Widgets API
  description: the-widgets-api-
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