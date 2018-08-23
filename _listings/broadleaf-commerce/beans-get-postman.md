{
  "info": {
    "name": "Broadleaf Commerce API Get Beans",
    "_postman_id": "dbdbb4de-432d-4213-814b-9f52e55f414f",
    "description": "Get beans.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Auditevents",
      "item": [
        {
          "id": "bf7c985d-e524-4137-8f4d-4e3a19b9287b",
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
              "id": "5a3197f4-9d76-4008-85f0-6d09f4fde49a"
            }
          ]
        },
        {
          "id": "855d20d7-fb24-4c8d-b485-db5bef575bd0",
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
              "id": "11dc9073-5309-4b9b-a7bf-f1422caff2bc"
            }
          ]
        }
      ]
    },
    {
      "name": "Autoconfig",
      "item": [
        {
          "id": "f22141aa-2c58-4127-9f0f-e8bff7a3a1ea",
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
              "id": "d3a74a8d-8b2a-4e40-8817-c64a7c01c61a"
            }
          ]
        },
        {
          "id": "f65614dd-0bcd-47c4-ac30-c9322c64441e",
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
              "id": "f745f75d-2bee-474c-988c-aec549be1cb5"
            }
          ]
        }
      ]
    },
    {
      "name": "Beans",
      "item": [
        {
          "id": "0492081d-609f-4620-9619-229fec6a021b",
          "name": "getBeans",
          "request": {
            "url": "http://demo.broadleafcommerce.org/api/v1/beans",
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
            "description": "Get beans."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32e80f43-18f1-4e8b-8920-eec50872c275"
            }
          ]
        }
      ]
    }
  ]
}