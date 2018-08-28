swagger: "2.0"
x-collection-name: TigerText
x-complete: 1
info:
  title: TigerConnect User API
  description: the-user-system-for-tigerconnect-messaging-platform-
  termsOfService: http://www.tigertext.com/developer-terms-of-use
  contact:
    name: TigerText
    url: http://www.tigertext.com/supportform/
    email: info@tigertext.com
  version: v2
host: developer.tigertext.me
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /message/typing/{recipient_address}/:
    delete:
      summary: Notify a recipient that the User is no longer typing in a conversation.
      description: Notify a recipient that the User is no longer typing in a conversation.
        The recipient is either another User or Group using address encoding.
      operationId: deleteMessageTyping
      x-api-path-slug: messagetypingrecipient-address-delete
      parameters:
      - in: path
        name: recipient_address
        description: The recipient address
      responses:
        200:
          description: OK
      tags:
      - Message
      - Typing
      - Recipient
      - Address