---
swagger: "2.0"
x-collection-name: StatusPage.io
x-complete: 0
info:
  title: StatusPage.io Get a list of all components
  version: 1.0.0
  description: Get a list of all components
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /pages/[page_id]/components.json:
    get:
      summary: Get a list of all components
      description: Get a list of all components
      operationId: get-a-list-of-all-components
      x-api-path-slug: pagespage-idcomponents-json-get
      responses:
        200:
          description: OK
      tags:
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