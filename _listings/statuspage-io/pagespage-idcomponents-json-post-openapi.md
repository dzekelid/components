---
swagger: "2.0"
x-collection-name: StatusPage.io
x-complete: 0
info:
  title: StatusPage.io Create a component
  version: 1.0.0
  description: Create a component
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
    post:
      summary: Create a component
      description: Create a component
      operationId: create-a-component
      x-api-path-slug: pagespage-idcomponents-json-post
      parameters:
      - in: query
        name: component[description]
        description: The description of the component
        type: string
      - in: query
        name: component[group_id]
        description: The id of the parent component (optional, only 1 level of nesting)
        type: string
      - in: query
        name: component[name]
        description: The name of the component
        type: string
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