swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calls/broadcasts/{id}/recipients:
    post:
      summary: Add recipients to a call broadcast
      description: Use this API to add the recipients to an existing voice broadcast.
        Post a list of Recipient objects to be added to the voice broadcast campaign.
        These contacts will not go through validation process, and will be acted upon
        as they are added. Recipients may be added as a list of contact ids, or list
        of numbers
      operationId: addCallBroadcastRecipients
      x-api-path-slug: callsbroadcastsidrecipients-post
      parameters:
      - in: body
        name: body
        description: A list of CallRecipient objects
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a call broadcast
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Recipients
  /texts/broadcasts/{id}/recipients:
    post:
      summary: Add recipients to a text broadcast
      description: Use this API to add recipients to a text broadcast which is already
        created. Post a list of Recipient objects to be immediately added to the text
        broadcast campaign. These contacts will not go through validation process,
        and will be acted upon as they are added. Recipients may be added as a list
        of contact ids, or list of numbers
      operationId: addTextBroadcastRecipients
      x-api-path-slug: textsbroadcastsidrecipients-post
      parameters:
      - in: body
        name: body
        description: A list of the TextRecipient objects
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a text broadcast
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
      - Recipients