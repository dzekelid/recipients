---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Update a recipient
  description: Updates a recipient that is assigned to a folder. The ID of the recipient
    must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/newsletters/folders/{folderId}/recipients:
    get:
      summary: List all recipients of a folder
      description: Lists all recipients of a folder. The ID of the folder must be
        specified.
      operationId: getRestNewslettersFoldersFolderRecipients
      x-api-path-slug: restnewslettersfoldersfolderidrecipients-get
      parameters:
      - in: path
        name: folderId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Recipients
      - Of
      - Folder
  /rest/newsletters/list_recipients:
    get:
      summary: List recipients
      description: List recipients.
      operationId: getRestNewslettersListRecipients
      x-api-path-slug: restnewsletterslist-recipients-get
      parameters:
      - in: query
        name: columns
        description: Filter that restricts the search result to specific columns
      - in: query
        name: folderId
        description: Filter that restricts the search result to a specific folderId
      - in: query
        name: isConfirmed
        description: Filter that restricts the search result to confirmed recipients
      - in: query
        name: itemsPerPage
        description: The number of orders to be displayed per page
      - in: query
        name: page
        description: The page to get
      - in: query
        name: with
        description: Load additional relations for a Recipient
      responses:
        200:
          description: OK
      tags:
      - List
      - Recipients
  /rest/newsletters/recipients:
    delete:
      summary: Delete recipients
      description: Delete recipients.
      operationId: deleteRestNewslettersRecipients
      x-api-path-slug: restnewslettersrecipients-delete
      responses:
        200:
          description: OK
      tags:
      - Recipients
    get:
      summary: List recipients of a folder
      description: List recipients of a folder.
      operationId: getRestNewslettersRecipients
      x-api-path-slug: restnewslettersrecipients-get
      parameters:
      - in: query
        name: email
        description: Filter that restricts the search result to the email address
          of the recipient
      - in: query
        name: folderId
        description: Filter that restricts the search result to the folder ID
      - in: query
        name: recipientId
        description: Filter that restricts the search result to the recipient ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Recipients
      - Of
      - Folder
    post:
      summary: Create a recipient
      description: Create a recipient.
      operationId: postRestNewslettersRecipients
      x-api-path-slug: restnewslettersrecipients-post
      parameters:
      - in: body
        name: /rest/newsletters/recipients
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: email
        description: The email address of the recipient
      - in: query
        name: firstName
        description: The first name of the recipient
      - in: query
        name: folderIds
        description: The IDs of the newsletter folders
      - in: query
        name: ignoreVisibility
        description: Value that indicates if the REST call considers folders without
          visibility
      - in: query
        name: ipAddress
        description: The IP address from where the customer has confirmed the newsletter
      - in: query
        name: isFrontend
        description: Value that indicates if the REST call was retrieved from the
          front end
      - in: query
        name: lastName
        description: The last name of the recipient
      responses:
        200:
          description: OK
      tags:
      - Recipient
  /rest/newsletters/recipients/{recipientId}:
    delete:
      summary: Delete a recipient
      description: Deletes a recipient. The ID of the recipient must be specified.
      operationId: deleteRestNewslettersRecipientsRecipient
      x-api-path-slug: restnewslettersrecipientsrecipientid-delete
      parameters:
      - in: path
        name: recipientId
      responses:
        200:
          description: OK
      tags:
      - Recipient
    get:
      summary: List a recipient
      description: Lists a recipient. The ID of the recipient must be specified.
      operationId: getRestNewslettersRecipientsRecipient
      x-api-path-slug: restnewslettersrecipientsrecipientid-get
      parameters:
      - in: path
        name: recipientId
      - in: query
        name: recipientsId
        description: The ID of the newsletter folder
      responses:
        200:
          description: OK
      tags:
      - List
      - Recipient
    put:
      summary: Update a recipient
      description: Updates a recipient that is assigned to a folder. The ID of the
        recipient must be specified.
      operationId: putRestNewslettersRecipientsRecipient
      x-api-path-slug: restnewslettersrecipientsrecipientid-put
      parameters:
      - in: body
        name: /rest/newsletters/recipients/{recipientId}
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: birthday
        description: The customer birthday as Date string (e
      - in: query
        name: email
        description: The email address of the newsletter recipient
      - in: query
        name: firstName
        description: The first name of the newsletter recipient
      - in: query
        name: folderId
        description: The ID of the newsletter folder
      - in: query
        name: folderIds
        description: 'DEPRECATED: The IDs of the newsletter folders'
      - in: query
        name: gender
        description: 'The gender of the customer, one of the following values: m,f'
      - in: query
        name: ipAddress
        description: The IP address from where the customer has confirmed the newsletter
      - in: query
        name: lastName
        description: The last name of the newsletter recipient
      - in: path
        name: recipientId
      responses:
        200:
          description: OK
      tags:
      - Recipient
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