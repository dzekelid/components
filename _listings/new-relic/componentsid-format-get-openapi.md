---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Get Components  . Format
  version: 1.0.0
  description: |-
    This API endpoint returns a single component, identified by its ID.

    See our documentation for a discussion on listing components by ID.
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /components/{id}.{format}:
    get:
      summary: Get Components  . Format
      description: |-
        This API endpoint returns a single component, identified by its ID.

        See our documentation for a discussion on listing components by ID.
      operationId: getComponents.Format
      x-api-path-slug: componentsid-format-get
      parameters:
      - in: path
        name: id
        description: Plugin ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Components
      - ""
      - .
      - Format
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