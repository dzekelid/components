---
swagger: "2.0"
x-collection-name: Azure Application Insights
x-complete: 1
info:
  title: Application Insights API
  description: application-insights-in-preview-is-an-allinone-telemetry-solution-that-can-help-you-detect-issues-triage-impact-and-solve-problems-in-your-web-apps-and-services-it-provides-deep-diagnostics-and-realtime-insights-while-being-a-seamless-part-of-your-alm-processes-through-visual-studio-visual-studio-team-services-and-azure-diagnostics-integrations-it-supports-aspnet-j2ee-and-most-of-the-popular-web-technologies-for-web-apps-on-azure-or-on-your-own-servers
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/providers/microsoft.insights/components:
    get:
      summary: List Components
      description: Gets a list of all Application Insights components within a subscription.
      operationId: Components_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftinsightscomponents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Components
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/components:
    get:
      summary: List Components By Resource Group
      description: Gets a list of Application Insights components within a resource
        group.
      operationId: Components_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftinsightscomponents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Components
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/components/{resourceName}:
    delete:
      summary: Delete Components
      description: Deletes an Application Insights component.
      operationId: Components_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftinsightscomponentsresourcename-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Components
    get:
      summary: Get Components
      description: Returns an Application Insights component.
      operationId: Components_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftinsightscomponentsresourcename-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Components
    put:
      summary: Create or Update Components
      description: 'Creates (or updates) an Application Insights component. Note:
        You cannot specify a different value for InstrumentationKey nor AppId in the
        Put operation.'
      operationId: Components_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftinsightscomponentsresourcename-put
      parameters:
      - in: body
        name: InsightProperties
        description: Properties that need to be specified to create an Application
          Insights component
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Components
    patch:
      summary: Update Components Tags
      description: Updates an existing component's tags. To update other fields use
        the CreateOrUpdate method.
      operationId: Components_UpdateTags
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftinsightscomponentsresourcename-patch
      parameters:
      - in: body
        name: ComponentTags
        description: Updated tag information to set into the component instance
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Components
---