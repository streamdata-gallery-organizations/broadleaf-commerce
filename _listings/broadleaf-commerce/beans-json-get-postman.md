{
  "info": {
    "name": "Broadleaf Commerce API Get Beans",
    "_postman_id": "acdb373f-82d8-42cf-a79e-c0bc1efbcb70",
    "description": "Get beans.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Auditevents",
      "item": [
        {
          "id": "93fa4751-3f41-4099-952e-9983ff3e2303",
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
              "id": "669ce110-44dd-4d16-b1ef-4b903d6b228b"
            }
          ]
        },
        {
          "id": "d7ebb0bf-aec8-4f21-8e4b-7aae3bd2545b",
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
              "id": "8ad682c7-2d79-4889-9950-de38fbf672d1"
            }
          ]
        }
      ]
    },
    {
      "name": "Autoconfig",
      "item": [
        {
          "id": "c6695b37-c0c0-48e1-990c-43f8d703b5b9",
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
              "id": "c242a364-b69c-494f-8675-a643e6d90fdb"
            }
          ]
        },
        {
          "id": "e01e8af4-9d75-4da0-8d4a-74d1f39d1a12",
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
              "id": "5bf13803-3101-49c7-b531-ea277ef8cbf1"
            }
          ]
        }
      ]
    },
    {
      "name": "Beans",
      "item": [
        {
          "id": "c9c34fed-8086-4b3f-8984-ad6ffc80119d",
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
              "id": "d08363d9-d446-41e0-9374-f7f373299a9d"
            }
          ]
        },
        {
          "id": "339aabff-a07d-4723-8c05-da0c8b370cf5",
          "name": "getBeans.json",
          "request": {
            "url": "http://demo.broadleafcommerce.org/api/v1/beans.json",
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
              "id": "6592821a-09a4-4741-a939-d15d59e70676"
            }
          ]
        }
      ]
    }
  ]
}