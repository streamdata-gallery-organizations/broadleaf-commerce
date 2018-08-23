---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Get Beans
  description: Get beans.
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /auditevents:
    get:
      summary: Get Auditevents
      description: Get auditevents.
      operationId: getAuditevents
      x-api-path-slug: auditevents-get
      parameters:
      - in: query
        name: after
        description: after
      - in: query
        name: principal
        description: principal
      - in: query
        name: type
        description: type
      responses:
        200:
          description: OK
      tags:
      - Auditevents
  /auditevents.json:
    get:
      summary: Get Auditevents
      description: Get auditevents.
      operationId: getAuditevents.json
      x-api-path-slug: auditevents-json-get
      parameters:
      - in: query
        name: after
        description: after
      - in: query
        name: principal
        description: principal
      - in: query
        name: type
        description: type
      responses:
        200:
          description: OK
      tags:
      - Auditevents
  /autoconfig:
    get:
      summary: Get Autoconfig
      description: Get autoconfig.
      operationId: getAutoconfig
      x-api-path-slug: autoconfig-get
      responses:
        200:
          description: OK
      tags:
      - Autoconfig
  /autoconfig.json:
    get:
      summary: Get Autoconfig
      description: Get autoconfig.
      operationId: getAutoconfig.json
      x-api-path-slug: autoconfig-json-get
      responses:
        200:
          description: OK
      tags:
      - Autoconfig
  /beans:
    get:
      summary: Get Beans
      description: Get beans.
      operationId: getBeans
      x-api-path-slug: beans-get
      responses:
        200:
          description: OK
      tags:
      - Beans
  /beans.json:
    get:
      summary: Get Beans
      description: Get beans.
      operationId: getBeans.json
      x-api-path-slug: beans-json-get
      responses:
        200:
          description: OK
      tags:
      - Beans
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