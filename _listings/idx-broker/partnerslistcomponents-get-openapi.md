---
swagger: "2.0"
x-collection-name: IDX Broker
x-complete: 0
info:
  title: IDX Broker Get Partners List Components
  description: This is a simple, access anywhere, method for getting a list of all
    API components available.
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
  /mls/listcomponents:
    get:
      summary: Get Mls List Components
      description: This is a simple, access anywhere, method for getting a list of
        all API components available.
      operationId: MlsListcomponentsGet
      x-api-path-slug: mlslistcomponents-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - List
      - Components
  /leads/listcomponents:
    get:
      summary: Get Leads List Components
      description: This is a simple, access anywhere, method for getting a list of
        all API components available.
      operationId: LeadsListcomponentsGet
      x-api-path-slug: leadslistcomponents-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - List
      - Components
  /partners/listcomponents:
    get:
      summary: Get Partners List Components
      description: This is a simple, access anywhere, method for getting a list of
        all API components available.
      operationId: PartnersListcomponentsGet
      x-api-path-slug: partnerslistcomponents-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - List
      - Components
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