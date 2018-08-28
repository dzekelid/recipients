---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List all recipients of a folder
  description: Lists all recipients of a folder. The ID of the folder must be specified.
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