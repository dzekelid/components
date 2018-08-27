---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get project components
  description: |-
    Returns all components existing in a single project. See the [Get project components paginated](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-project-projectIdOrKey-component-get) resource if you want to get a full list of components with pagination.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ project permission.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/project/{projectIdOrKey}/component:
    get:
      summary: Get project components paginated
      description: |-
        Returns a [paginated](https://developer.atlassian.com/cloud/jira/platform/rest/#pagination) representation of all components existing in a single project. See the [Get project components](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-project-projectIdOrKey-components-get) resource if you want to get a full list of versions without pagination.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ project permission.
      operationId: com.atlassian.jira.rest.v2.issue.ProjectResource.getProjectComponentsPaginated_get
      x-api-path-slug: api2projectprojectidorkeycomponent-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of components to return per page
      - in: query
        name: orderBy
        description: '[Order](https://developer'
      - in: path
        name: projectIdOrKey
        description: The project ID or project key (case sensitive)
      - in: query
        name: query
        description: Filter the results using a literal string
      - in: query
        name: startAt
        description: The starting index of the returned list of components
      responses:
        200:
          description: OK
      tags:
      - Project
      - Components
      - Paginated
  /api/2/project/{projectIdOrKey}/components:
    get:
      summary: Get project components
      description: |-
        Returns all components existing in a single project. See the [Get project components paginated](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-project-projectIdOrKey-component-get) resource if you want to get a full list of components with pagination.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ project permission.
      operationId: com.atlassian.jira.rest.v2.issue.ProjectResource.getProjectComponents_get
      x-api-path-slug: api2projectprojectidorkeycomponents-get
      parameters:
      - in: path
        name: projectIdOrKey
        description: The project ID or project key (case sensitive)
      responses:
        200:
          description: OK
      tags:
      - Project
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