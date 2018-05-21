---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Get Components Component  Metrics Data. Format
  version: 1.0.0
  description: "This API endpoint returns a list of values for each of the requested
    metrics. The list of available metrics\ncan be returned using the Metric Name
    API endpoint.\n\nMetric data can be filtered by a number of parameters, including
    multiple names and values, and by time range.\nMetric names and values will be
    matched intelligently in the background.\n\nYou can also retrieve a summarized
    data point across the entire time range selected by using the summarize\nparameter.\n\nSee
    our documentation for a discussion on \noutput pagination,  time range \nrelated
    considerations, and for examples of requesting and using metric values."
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /components.{format}:
    get:
      summary: Get Components. Format
      description: |-
        This API endpoint returns a list of the plugin components associated with your New Relic account.

        Plugins can be filtered by their name, the list of component IDs or a plugin ID.

        See our documentation for a discussion on  listing components
        and  output pagination.
      operationId: getComponents.Format
      x-api-path-slug: componentsformat-get
      parameters:
      - in: query
        name: filter[ids]
        description: Filter components by ids
        type: list
      - in: query
        name: filter[name]
        description: Filter components by name
        type: string
      - in: query
        name: filter[plugin_id]
        description: Filter components by the plugin
        type: integer
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Components.
      - Format
  /components/{id}.{format}:
    get:
      summary: Get Components  . Format
      description: |-
        This API endpoint returns a single component, identified by its ID.

        See our documentation for a discussion on listing components by ID.
      operationId: getComponents.Format
      x-api-path-slug: componentsidformat-get
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
  /components/{component_id}/metrics.{format}:
    get:
      summary: Get Components Component  Metrics. Format
      description: |-
        Return a list of known metrics and their value names for the given resource.

        See our documentation for a discussion
        on  output pagination
        and for examples of requesting and using metric values.
      operationId: getComponentsComponentMetrics.Format
      x-api-path-slug: componentscomponent-idmetricsformat-get
      parameters:
      - in: path
        name: component_id
        description: Component ID
        type: integer
      - in: query
        name: cursor
        description: Cursor for next page (replacing page param)
        type: string
      - in: query
        name: name
        description: Filter metrics by name
        type: string
      - in: query
        name: page
        description: Pagination index (will be deprecated)
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Components
      - Component
      - ""
      - Metrics.
      - Format
  /components/{component_id}/metrics/data.{format}:
    get:
      summary: Get Components Component  Metrics Data. Format
      description: "This API endpoint returns a list of values for each of the requested
        metrics. The list of available metrics\ncan be returned using the Metric Name
        API endpoint.\n\nMetric data can be filtered by a number of parameters, including
        multiple names and values, and by time range.\nMetric names and values will
        be matched intelligently in the background.\n\nYou can also retrieve a summarized
        data point across the entire time range selected by using the summarize\nparameter.\n\nSee
        our documentation for a discussion on \noutput pagination,  time range \nrelated
        considerations, and for examples of requesting and using metric values."
      operationId: getComponentsComponentMetricsData.Format
      x-api-path-slug: componentscomponent-idmetricsdataformat-get
      parameters:
      - in: path
        name: component_id
        description: Component ID
        type: integer
      - in: query
        name: from
        description: Retrieve metrics after this time
        type: time
      - in: query
        name: names
        description: Retrieve specific metrics by name
        type: array
      - in: query
        name: period
        description: Period of timeslices in seconds
        type: integer
      - in: query
        name: raw
        description: Return unformatted raw values
        type: boolean
      - in: query
        name: summarize
        description: Summarize the data
        type: boolean
      - in: query
        name: to
        description: Retrieve metrics before this time
        type: time
      - in: query
        name: values
        description: Retrieve specific metric values
        type: array
      responses:
        200:
          description: OK
      tags:
      - Components
      - Component
      - ""
      - Metrics
      - Data.
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