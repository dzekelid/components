---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Remove a bundle component
  description: Removes a component from a bundle. The bundle ID must be specified.
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
    put:
      summary: Update item set components
      description: Update item set components.
      operationId: putRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponents-put
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
  /rest/items/{id}/variations/{variationId}/variation_bundles:
    get:
      summary: List bundle components
      description: List all components of a bundle. The ID of the item and the ID
        of the variation to which bundle components were added must be specified.
      operationId: getRestItemsVariationsVariationVariationBundles
      x-api-path-slug: restitemsidvariationsvariationidvariation-bundles-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Bundle
      - Components
  /rest/item_sets/{setId}/components/{id}:
    delete:
      summary: Delete an item set component
      description: Deletes an item set component. The item set component ID of the
        item set component must be specified.
      operationId: deleteRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponentsid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Component
    get:
      summary: Get an item set component
      description: Get an item set component.
      operationId: getRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponentsid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Component
    put:
      summary: Update an item set component
      description: Update an item set component.
      operationId: putRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponentsid-put
      parameters:
      - in: path
        name: id
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Component
  /rest/items/{id}/variations/{variationId}/variation_bundles/{bundleId}:
    delete:
      summary: Remove a bundle component
      description: Removes a component from a bundle. The bundle ID must be specified.
      operationId: deleteRestItemsVariationsVariationVariationBundlesBundle
      x-api-path-slug: restitemsidvariationsvariationidvariation-bundlesbundleid-delete
      parameters:
      - in: path
        name: bundleId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Bundle
      - Component
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