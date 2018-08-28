---
swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 0
info:
  title: AXA Assistance Sends a prescription to its recipient
  description: Sends a prescription to its recipient
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/v1/medical_consultations/{medical_consultation_id}/prescriptions/{prescription_id}/send:
    post:
      summary: Sends a prescription to its recipient
      description: Sends a prescription to its recipient
      operationId: postServiceV1Medical_consultationsMedical_consultation_idPrescriptionsPrescription_idSend
      x-api-path-slug: servicev1medical-consultationsmedical-consultation-idprescriptionsprescription-idsend-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: medical_consultation_id
        description: ID of the medical consultation
      - in: path
        name: prescription_id
        description: ID of the prescription
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Sendsprescription
      - to
      - itAssistance
      - recipient
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