---
name: New Relic
x-slug: new-relic
description: New Relic offers SaaS Software Analytics Platform that offers Application
  Performance Management and Real User Monitoring for Cloud and Data Center deployed
  web applications implemented in Ruby, Java, .NET, Python, PHP, Node.js. New Relic
  also offers mobile monitoring solutions for iOS and Android applications.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
x-kinRank: "8"
x-alexaRank: ""
tags: Components
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/components/master/_listings/new-relic/apis.md
specificationVersion: "0.14"
apis:
- name: New Relic Get Components. Format
  x-api-slug: new-relic
  description: |-
    This API endpoint returns a list of the plugin components associated with your New Relic account.

    Plugins can be filtered by their name, the list of component IDs or a plugin ID.

    See our documentation for a discussion on  listing components
    and  output pagination.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
  humanURL: https://newrelic.com/
  baseURL: https:///v2///components.{format}
  tags: Components., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/components/master/_listings/new-relic/componentsformat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/components/master/_listings/new-relic/componentsformat-get-openapi.md
- name: New Relic Get Components  . Format
  x-api-slug: new-relic
  description: |-
    This API endpoint returns a single component, identified by its ID.

    See our documentation for a discussion on listing components by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
  humanURL: https://newrelic.com/
  baseURL: https:///v2///components/{id}.{format}
  tags: Components, , ., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/components/master/_listings/new-relic/componentsidformat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/components/master/_listings/new-relic/componentsidformat-get-openapi.md
- name: New Relic Get Components Component  Metrics. Format
  x-api-slug: new-relic
  description: |-
    Return a list of known metrics and their value names for the given resource.

    See our documentation for a discussion
    on  output pagination
    and for examples of requesting and using metric values.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
  humanURL: https://newrelic.com/
  baseURL: https:///v2///components/{component_id}/metrics.{format}
  tags: Components, Component, , Metrics., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/components/master/_listings/new-relic/componentscomponent-idmetricsformat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/components/master/_listings/new-relic/componentscomponent-idmetricsformat-get-openapi.md
- name: New Relic Get Components Component  Metrics Data. Format
  x-api-slug: new-relic
  description: "This API endpoint returns a list of values for each of the requested
    metrics. The list of available metrics\ncan be returned using the Metric Name
    API endpoint.\n\nMetric data can be filtered by a number of parameters, including
    multiple names and values, and by time range.\nMetric names and values will be
    matched intelligently in the background.\n\nYou can also retrieve a summarized
    data point across the entire time range selected by using the summarize\nparameter.\n\nSee
    our documentation for a discussion on \noutput pagination,  time range \nrelated
    considerations, and for examples of requesting and using metric values."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
  humanURL: https://newrelic.com/
  baseURL: https:///v2///components/{component_id}/metrics/data.{format}
  tags: Components, Component, , Metrics, Data., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/components/master/_listings/new-relic/componentscomponent-idmetricsdataformat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/components/master/_listings/new-relic/componentscomponent-idmetricsdataformat-get-openapi.md
- name: New Relic
  x-api-slug: new-relic
  description: New Relic offers SaaS Software Analytics Platform that offers Application
    Performance Management and Real User Monitoring for Cloud and Data Center deployed
    web applications implemented in Ruby, Java, .NET, Python, PHP, Node.js. New Relic
    also offers mobile monitoring solutions for iOS and Android applications.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Components
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/components/master/_listings/new-relic/openapi.md
x-common:
- type: x-blog
  url: https://blog.newrelic.com/
- type: x-blog-rss
  url: https://blog.newrelic.com/feed/
- type: x-developer
  url: https://rpm.newrelic.com/api/explore/
- type: x-github
  url: https://github.com/newrelic
- type: x-twitter
  url: https://twitter.com/NewRelic
- type: x-website
  url: https://newrelic.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---