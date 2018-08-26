{
  "info": {
    "name": "Broadleaf Commerce API Get Auditevents",
    "_postman_id": "0aff57d7-2423-43b0-b6fa-a34f6b9d174f",
    "description": "Get auditevents.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Auditevents",
      "item": [
        {
          "id": "a67bb86d-0ea5-473a-9e1d-6f39fd9df9da",
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
              "id": "b6aefe32-a9c1-4183-aa44-24cbe37d61ed"
            }
          ]
        }
      ]
    }
  ]
}