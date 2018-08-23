{
  "info": {
    "name": "Broadleaf Commerce API Get Autoconfig",
    "_postman_id": "4eebe89c-9bff-47da-bc6d-06fc6b803f2a",
    "description": "Get autoconfig.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Auditevents",
      "item": [
        {
          "id": "d3eee12f-7b61-446c-9d0f-300508624cba",
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
              "id": "80c51979-845e-468f-a055-cd1ca23c1e98"
            }
          ]
        },
        {
          "id": "04a53b1a-c6dd-4272-971a-242a4184fa7a",
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
              "id": "13853eaa-7412-49a6-8175-174d14e46e4c"
            }
          ]
        }
      ]
    },
    {
      "name": "Autoconfig",
      "item": [
        {
          "id": "4a5d9336-1657-4af9-9c42-94b44c54ed90",
          "name": "getAutoconfig",
          "request": {
            "url": "http://demo.broadleafcommerce.org/api/v1/autoconfig",
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
            "description": "Get autoconfig."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e099b27e-1696-4264-b317-2616ae9bb30d"
            }
          ]
        }
      ]
    }
  ]
}