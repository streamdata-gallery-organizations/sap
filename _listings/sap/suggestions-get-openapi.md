---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Translation Hub The suggestion resource enables you to get suggestions
    for short texts during the development process.
  description: Provides suggestions for short texts based on complete or partial texts
    and their translations. You can, for example, use the suggestion resource to propose
    texts while you type texts in a development environment. The texts that the resource
    proposes are already available in additional languages in the multilingual text
    repository (MLTR).
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
  /languages:
    get:
      summary: Languages that SAP Translation Hub supports.
      description: Returns a list of the languages that SAP Translation Hub supports.
        You can also check whether a particualr language is available in SAP Translation
        Hub.
      operationId: returns-a-list-of-the-languages-that-sap-translation-hub-supports-you-can-also-check-whether-a-parti
      x-api-path-slug: languages-get
      parameters:
      - in: header
        name: Content-Type
        description: Specifies the nature of the data in the body so that the receiving
          agent can process the data accordingly
      - in: query
        name: search
        description: Determines whether a particular language is available in SAP
          Translation Hub
      responses:
        200:
          description: Successful response
      tags:
      - Languages
      - That
      - SAP
      - Translation
      - Hub
      - Supports
  /suggestions:
    get:
      summary: The suggestion resource enables you to get suggestions for short texts
        during the development process.
      description: Provides suggestions for short texts based on complete or partial
        texts and their translations. You can, for example, use the suggestion resource
        to propose texts while you type texts in a development environment. The texts
        that the resource proposes are already available in additional languages in
        the multilingual text repository (MLTR).
      operationId: provides-suggestions-for-short-texts-based-on-complete-or-partial-texts-and-their-translations-you-c
      x-api-path-slug: suggestions-get
      parameters:
      - in: header
        name: Content-Type
        description: Specifies the nature of the data in the body so that the receiving
          agent can process the data accordingly
      - in: query
        name: domain
        description: Searches for texts in the specified domain(s) or domain group(s)
      - in: query
        name: language
        description: Allows you to search for a text that has translations in the
          specified language(s)
      - in: query
        name: maxLength
        description: Searches for texts up to the specified number of characters
      - in: query
        name: search
        description: Allows you to search for a text in SAP Translation Hub in English
      - in: query
        name: searchLanguage
        description: Allows you to search for a text in any of the languages that
          SAP Translation Hub supports
      - in: query
        name: texttype
        description: Allows you to search for a text that is assigned to one or more
          text types
      responses:
        200:
          description: Successful response
      tags:
      - The
      - Suggestion
      - Resource
      - Enables
      - You
      - To
      - Get
      - Suggestionsshort
      - Texts
      - During
      - Development
      - Process
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