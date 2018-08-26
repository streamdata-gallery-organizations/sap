---
name: SAP
x-slug: sap
description: Get software and technology solutions from SAP, the leader in business
  applications.  Run simple with the best in cloud, analytics, mobile and IT solutions.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
x-kinRank: "8"
x-alexaRank: "1965"
tags: SAP
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/apis.md
specificationVersion: "0.14"
apis:
- name: SAP Translation Hub - SAP product domains
  x-api-slug: domains-get
  description: SAP product terminology is organized by domains. Domains are used in
    the translation process to determine the correct terminology for a given application.
    <br> This resource returns a list of the domains and domain groups that are available
    in SAP Translation Hub.<br> You can combine the domain resource with the translation
    resource to more accurately reflect the subject area of your texts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://sandbox.api.sap.com//translationhub/api/v1
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/domains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/domains-get-openapi.md
- name: SAP Translation Hub - Languages that SAP Translation Hub supports.
  x-api-slug: languages-get
  description: Returns a list of the languages that SAP Translation Hub supports.
    You can also check whether a particualr language is available in SAP Translation
    Hub.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://sandbox.api.sap.com//translationhub/api/v1
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/languages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/languages-get-openapi.md
- name: SAP Translation Hub - The suggestion resource enables you to get suggestions
    for short texts during the development process.
  x-api-slug: suggestions-get
  description: Provides suggestions for short texts based on complete or partial texts
    and their translations. You can, for example, use the suggestion resource to propose
    texts while you type texts in a development environment. The texts that the resource
    proposes are already available in additional languages in the multilingual text
    repository (MLTR).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://sandbox.api.sap.com//translationhub/api/v1
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/suggestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/suggestions-get-openapi.md
- name: SAP Translation Hub - Returns a list of the text types available in SAP Translation
    Hub.
  x-api-slug: texttypes-get
  description: In SAP products, short texts, such as those used on user interfaces
    (UIs), are characterized by various text types. The type of a specific text is
    determined by the UI element that it describes. For example,  button texts are
    described by the text type ```XBUT```. <br> The text type resource returns a list
    of the text types that are available in SAP Translation Hub. You can combine the
    '/text type' resource with the '/suggestion' resource to narrow down the results
    of the suggestion resource.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://sandbox.api.sap.com//translationhub/api/v1
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/texttypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/texttypes-get-openapi.md
x-common:
- type: x-website
  url: https://www.sap.com/index.html
- type: x-api-gallery
  url: http://santander.bank.api.gallery.streamdata.io
- type: x-api-stack
  url: http://sap.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/sap-canada
- type: x-developer
  url: https://api.sap.com/
- type: x-github
  url: https://github.com/sap
- type: x-twitter
  url: https://twitter.com/SAP
- type: x-website
  url: https://www.sap.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---