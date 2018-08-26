---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Create item set components
  description: Create item set components.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
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
  /rest/item_sets/{setId}/components:
    delete:
      summary: Delete item set components
      description: Delete item set components.
      operationId: deleteRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponents-delete
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Components
    get:
      summary: List item set components of an item set
      description: Lists the item set components of an item set. The ID of the item
        set must be specified.
      operationId: getRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponents-get
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Set
      - Components
      - Of
      - Item
      - Set
    post:
      summary: Create item set components
      description: Create item set components.
      operationId: postRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponents-post
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
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