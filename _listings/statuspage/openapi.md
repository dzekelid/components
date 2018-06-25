---
swagger: "2.0"
x-collection-name: StatusPage
x-complete: 1
info:
  title: StatusPage.io
  version: 1.0.0
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
  /pages/[page_id]/components/[component_id].json:
    delete:
      summary: Delete a component
      description: Delete a component
      operationId: delete-a-component
      x-api-path-slug: pagespage-idcomponentscomponent-id-json-delete
      responses:
        200:
          description: OK
      tags:
      - Components
---