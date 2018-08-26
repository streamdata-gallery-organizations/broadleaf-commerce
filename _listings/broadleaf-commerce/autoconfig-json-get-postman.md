{
  "info": {
    "name": "Broadleaf Commerce API Get Autoconfig",
    "_postman_id": "2762d809-3e45-456a-9054-19a23a9f0ed7",
    "description": "Get autoconfig.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Auditevents",
      "item": [
        {
          "id": "dbe01b23-57ba-4b5e-bc44-991438758878",
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
              "id": "20efa57b-99e3-4dfa-8ee8-73ae7ef0d85c"
            }
          ]
        },
        {
          "id": "696039ec-c520-4863-9223-55e8435a3542",
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
              "id": "c36a23b8-868b-4de2-a5db-e0719b6640e5"
            }
          ]
        }
      ]
    },
    {
      "name": "Autoconfig",
      "item": [
        {
          "id": "f48a068c-cb00-4561-8480-5d6eacaf3d95",
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
              "id": "321abc8e-1225-43bd-8788-546e136651a2"
            }
          ]
        },
        {
          "id": "c12274b2-12f7-4d47-bda7-bf75ac877f11",
          "name": "getAutoconfig.json",
          "request": {
            "url": "http://demo.broadleafcommerce.org/api/v1/autoconfig.json",
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
              "id": "a24e0720-70c9-4829-8d0d-56c619c1cee6"
            }
          ]
        }
      ]
    }
  ]
}