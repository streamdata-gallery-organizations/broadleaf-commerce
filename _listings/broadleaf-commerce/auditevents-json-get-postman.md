{
  "info": {
    "name": "Broadleaf Commerce API Get Auditevents",
    "_postman_id": "2d6d57d7-ff9a-4683-8878-625f7d7789f5",
    "description": "Get auditevents.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Auditevents",
      "item": [
        {
          "id": "dc51571d-9580-4f68-a1bd-14cf577a4fc6",
          "name": "getAuditevents",
          "request": {
            "url": "http://demo.broadleafcommerce.org/api/v1/auditevents?after=%7B%7D&principal=%7B%7D&type=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get auditevents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "313564ab-7323-4b55-bfb8-a60516cd6dba"
            }
          ]
        },
        {
          "id": "30c235f4-a64e-4a5c-a19e-8bd5cc8727d1",
          "name": "getAuditevents.json",
          "request": {
            "url": "http://demo.broadleafcommerce.org/api/v1/auditevents.json?after=%7B%7D&principal=%7B%7D&type=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get auditevents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "961a02c3-dcaa-4d2f-969a-f57ad8da1376"
            }
          ]
        }
      ]
    }
  ]
}