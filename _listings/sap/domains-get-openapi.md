---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Translation Hub SAP product domains
  description: SAP product terminology is organized by domains. Domains are used in
    the translation process to determine the correct terminology for a given application.
    <br> This resource returns a list of the domains and domain groups that are available
    in SAP Translation Hub.<br> You can combine the domain resource with the translation
    resource to more accurately reflect the subject area of your texts.
  contact:
    name: SAP Translation Hub team
    email: translationhub@sap.com
  version: 1.0.0
host: sandbox.api.sap.com
basePath: /translationhub/api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /domains:
    get:
      summary: SAP product domains
      description: SAP product terminology is organized by domains. Domains are used
        in the translation process to determine the correct terminology for a given
        application. <br> This resource returns a list of the domains and domain groups
        that are available in SAP Translation Hub.<br> You can combine the domain
        resource with the translation resource to more accurately reflect the subject
        area of your texts.
      operationId: sap-product-terminology-is-organized-by-domains-domains-are-used-in-the-translation-process-to-deter
      x-api-path-slug: domains-get
      parameters:
      - in: header
        name: Content-Type
        description: Specifies the nature of the data in the body so that the receiving
          agent can process the data accordingly
      - in: query
        name: onlyGroups
        description: Shows a list of the domain groups that SAP Translation Hub supports
      - in: query
        name: search
        description: Shows whether a particular domain is available in SAP Translation
          Hub
      responses:
        200:
          description: Successful response
      tags:
      - SAP
      - Product
      - Domains
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