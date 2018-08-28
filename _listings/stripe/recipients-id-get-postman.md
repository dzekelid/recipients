{
  "info": {
    "name": "Stripe Get Recipients",
    "_postman_id": "92af7ea9-6176-45cd-8fe9-db04c50245f8",
    "description": "Retrieves the details of an existing recipient. You need only supply the unique recipient identifier that was returned upon recipient creation.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "recipients",
      "item": [
        {
          "id": "e6fa4c75-286c-4f06-aa6d-7b6602997c8a",
          "name": "getRecipients",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "recipients/:id"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the details of an existing recipient"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20654235-330b-4423-9041-915d4cb06403"
            }
          ]
        }
      ]
    }
  ]
}