---
name: SAP
x-slug: sap
description: Get software and technology solutions from SAP, the leader in business
  applications.  Run simple with the best in cloud, analytics, mobile and IT solutions.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
x-kinRank: "8"
x-alexaRank: "1965"
tags: SAP
created: "2018-08-31"
modified: "2018-08-31"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/apis.md
specificationVersion: "0.14"
apis:
- name: Manufacturing Network Customer APIs - Sends a callback message
  x-api-slug: callback-post
  description: |-
    Upon the receipt of an event, send a response in an async way to the event framework of Manufacturing Network.

    In the callback message, be sure to include the event ID. Add other information as appropriate.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/callback-post-openapi.md
- name: Manufacturing Network Customer APIs - Creates a collaboration room
  x-api-slug: collaborationrooms-post
  description: "Creates a collaboration room.  \nThe login user must be from a customer."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationrooms-post-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves a collaboration room
  x-api-slug: collaborationroomscollaborationroomid-get
  description: Retrieves the information of a collaboration room by its ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomid-get-openapi.md
- name: Manufacturing Network Customer APIs - Updates a collaboration room
  x-api-slug: collaborationroomscollaborationroomid-patch
  description: Updates a collaboration room.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomid-patch-openapi.md
- name: Manufacturing Network Customer APIs - Deletes a collaboration room
  x-api-slug: collaborationroomscollaborationroomid-delete
  description: |-
    Deletes a collaboration room
    The login user must be a collaboration lead for the customer and it must be a new or discarded collaboration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomid-delete-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves basic info of a collaboration
    room
  x-api-slug: collaborationroomscollaborationroomidbasic-get
  description: Retrieves the information of a collaboration room in a simplified form.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidbasic-get-openapi.md
- name: Manufacturing Network Customer APIs - Starts a collaboration
  x-api-slug: collaborationroomscollaborationroomidstart-post
  description: "Sets a collaboration in process.  \nThe collaboration must be a new
    collaboration."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidstart-post-openapi.md
- name: Manufacturing Network Customer APIs - Completes a collaboration
  x-api-slug: collaborationroomscollaborationroomidcomplete-post
  description: |-
    Sets a collaboration as completed
    - The login user must be a collaboration lead for the customer.
    - If there's already a supplier in the collaboration room, the collaboration must already or still be in process.
    - If there's already a completed collaboration with the same additive manufacturing supplier, part ID, and customer, this operation fails.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidcomplete-post-openapi.md
- name: Manufacturing Network Customer APIs - Discards a collaboration
  x-api-slug: collaborationroomscollaborationroomiddiscard-post
  description: "Sets a collaboration as discarded.  \nThe login user must be a collaboration
    lead for the customer and the collaboration must be in process or completed."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomiddiscard-post-openapi.md
- name: Manufacturing Network Customer APIs - Reopens a collaboration
  x-api-slug: collaborationroomscollaborationroomidreopen-post
  description: "Reopens a completed collaboration.  \nThe collaboration is set back
    to the status 'In Process'.\nThe login user must be a collaboration lead for the
    customer."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidreopen-post-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves documents in a collaboration
    room
  x-api-slug: collaborationroomscollaborationroomiddocuments-get
  description: Retrieves the information of all documents in a collaboration room,
    such as design files and specifications.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomiddocuments-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves a document
  x-api-slug: collaborationroomscollaborationroomiddocumentsfileid-get
  description: Retrieves the information of a document by its ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomiddocumentsfileid-get-openapi.md
- name: Manufacturing Network Customer APIs - Deletes a document
  x-api-slug: collaborationroomscollaborationroomiddocumentsfileid-delete
  description: "Deletes a document.  \nThe login user must be the one who uploaded
    the file."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomiddocumentsfileid-delete-openapi.md
- name: Manufacturing Network Customer APIs - Gets conversion info of a design file
  x-api-slug: collaborationroomscollaborationroomiddocumentsfileidconversion-get
  description: "Retrieves the information of the conversion event for a design file.\nA
    conversion event converts a design file into a VDS file.  \nSee a full list of
    supported formats in the [online help](https://help.sap.com/viewer/dmc-mn-app-help-customer/710ee60457ca457cbda854c363bcf71f.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomiddocumentsfileidconversion-get-openapi.md
- name: Manufacturing Network Customer APIs - Converts a design file
  x-api-slug: collaborationroomscollaborationroomiddocumentsfileidconversion-post
  description: |-
    Invokes a conversion event that converts a design file into a VDS file.

    See a full list of supported formats in the [online help](https://help.sap.com/viewer/dmc-mn-app-help-customer/710ee60457ca457cbda854c363bcf71f.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomiddocumentsfileidconversion-post-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves the production data
  x-api-slug: collaborationroomscollaborationroomidproductiondata-get
  description: Retrieves the production data in a collaboration room, including the
    currency, all the production options, and the initial pricings provided by the
    supplier.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidproductiondata-get-openapi.md
- name: Manufacturing Network Customer APIs - Creates a production option
  x-api-slug: collaborationroomscollaborationroomidproductiondata-post
  description: "Creates a new production option, providing the pricing information
    in the meantime.  \nThe login user must be a collaboration lead from the additive
    manufacturing supplier."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidproductiondata-post-openapi.md
- name: Manufacturing Network Customer APIs - Creates a production option without
    pricing
  x-api-slug: collaborationroomscollaborationroomidproductiondatabasic-post
  description: "Creates a new production option without an initial pricing.  \nThis
    endpoint is used by users from the additive manufactuirng supplier that're not
    collaboration leads."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidproductiondatabasic-post-openapi.md
- name: Manufacturing Network Customer APIs - Updates the pricing
  x-api-slug: collaborationroomscollaborationroomidproductiondataoriginalpricing-put
  description: "Updates the initial pricing for the customer's production option.
    \ \nThe login user must be a collaboration lead from an additive manufacturing
    supplier.  \nNote: The planned quantity is defined by the customer and not available
    for update by the supplier."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidproductiondataoriginalpricing-put-openapi.md
- name: Manufacturing Network Customer APIs - Updates the customer's production option
  x-api-slug: collaborationroomscollaborationroomidproductiondataoriginalrequirement-put
  description: "Updates the customer's production option.   \nThe login user must
    be from the customer."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidproductiondataoriginalrequirement-put-openapi.md
- name: Manufacturing Network Customer APIs - Updates a supplier's production option
  x-api-slug: collaborationroomscollaborationroomidproductiondataproductiondataid-put
  description: "Updates a production option proposed by the additive manufacturing
    supplier as well as the initial pricing for this option.  \nThe login user must
    be a collaboration lead from the additive manufacturing supplier."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidproductiondataproductiondataid-put-openapi.md
- name: Manufacturing Network Customer APIs - Deletes a supplier's production option
  x-api-slug: collaborationroomscollaborationroomidproductiondataproductiondataid-delete
  description: "Deletes a production option proposed by the additive manufacturing
    supplier. The initial pricing is deleted along with it.  \nThe login user must
    be from the additive manufacturing supplier."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidproductiondataproductiondataid-delete-openapi.md
- name: Manufacturing Network Customer APIs - Updates a supplier's production option
  x-api-slug: collaborationroomscollaborationroomidproductiondataproductiondataidbasic-put
  description: "Updates a production option proposed by the additive manufacturing
    supplier.    \nThis endpoint is used by users from the additive manufactuirng
    supplier that're not collaboration leads. The initial pricing cannot be updated."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidproductiondataproductiondataidbasic-put-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves the confirmed production option
  x-api-slug: collaborationroomscollaborationroomidproductiondataconfirmed-get
  description: Retrieves the production option confirmed as the finalized production
    requirements, and the initial pricing for it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidproductiondataconfirmed-get-openapi.md
- name: Manufacturing Network Customer APIs - Confirms a production option
  x-api-slug: collaborationroomscollaborationroomidproductiondataproductiondataidconfirm-post
  description: "Confirms a production option along with the initial pricing for it.
    \ \nThe production option might be proposed by the customer or the additive manufacturing
    supplier.   \nThe login user must be from the customer."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidproductiondataproductiondataidconfirm-post-openapi.md
- name: Manufacturing Network Customer APIs - Cancels the confirmation of a production
    option
  x-api-slug: collaborationroomscollaborationroomidproductiondataproductiondataidcancelconfirm-post
  description: "Undos the confirmation of a production option.  \nThe login user must
    be from the customer."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidproductiondataproductiondataidcancelconfirm-post-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves the thumbnail of a design
    file
  x-api-slug: collaborationroomscollaborationroomidthumbnails-get
  description: |-
    Retrieves the thumbnail information in a collaboration room.
    Each design file has a corresponding thumbnail file automatically generated.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidthumbnails-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves available collaboration room
    templates
  x-api-slug: collaborationtemplates-get
  description: Retrieves available collaboration room templates.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationtemplates-get-openapi.md
- name: Manufacturing Network Customer APIs - Downloads a file
  x-api-slug: documentscollaborationroomscollaborationroomiddownload-get
  description: Downloads a file from a collaboration room.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/documentscollaborationroomscollaborationroomiddownload-get-openapi.md
- name: Manufacturing Network Customer APIs - Uploads a file to a collaboration room
  x-api-slug: documentscollaborationroomscollaborationroomidupload-post
  description: Uploads a file to a collaboration room.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/documentscollaborationroomscollaborationroomidupload-post-openapi.md
- name: Manufacturing Network Customer APIs - Downloads the thumbnail of a design
    file
  x-api-slug: documentscollaborationroomscollaborationroomidthumbnaildownload-get
  description: Downloads the thumbnail selected as the icon for a collaboration room.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/documentscollaborationroomscollaborationroomidthumbnaildownload-get-openapi.md
- name: Manufacturing Network Customer APIs - Uploads a file to the temp folder
  x-api-slug: documentsorganizationsorganizationidtempupload-post
  description: Uploads a file to the temp folder for an organization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/documentsorganizationsorganizationidtempupload-post-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves all extensions
  x-api-slug: extensions-get
  description: "Retrieves all the extensions that have been registered with Manufacturing
    Network.  \nThese extensions are developed by Manufacturing Network customers
    or partners to enhance the functionality of the application."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/extensions-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves extensions available for use
  x-api-slug: extensionsavailable-get
  description: "Retrieves extensions that can be used during a collaboration.  \nA
    supplier enables an extension for collaboration by selecting it for use in the
    supplier profile."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/extensionsavailable-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves supplier profile master data
  x-api-slug: masterdata-get
  description: |-
    Retrieves master data such as processes and materials.
    Narrow down the result by specifying the master data types.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/masterdata-get-openapi.md
- name: Manufacturing Network Customer APIs - Creates an order
  x-api-slug: orders-post
  description: |-
    Creates an order for the part for which the customer and the supplier haven been colloabrating
    The order is based on the confirmed production option and pricing.
    The login user must be from the customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/orders-post-openapi.md
- name: Manufacturing Network Customer APIs - Adds a record to the order history
  x-api-slug: ordersordernumberhistory-post
  description: "Adds a record to the history of an order.   \nThe order number is
    sent in the message body of the Order Created event.  \nThe login user must be
    from the additive manufacturing supplier."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/ordersordernumberhistory-post-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves your own organization
  x-api-slug: organizationsself-get
  description: Retrieves the information of the login user's own organization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/organizationsself-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves organizations available for
    collaboration
  x-api-slug: organizationsvisible-get
  description: "Retrieves organizations in a specific business role that are available
    for collaboration.  \nThese organizations may have been approved for or blocked
    from collaboration, or they're still pending for approval.\nThe login user must
    be from a customer."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/organizationsvisible-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves an organization
  x-api-slug: organizationsorganizationid-get
  description: Retrieves an organization by its ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/organizationsorganizationid-get-openapi.md
- name: Manufacturing Network Customer APIs - Updates a supplier profile
  x-api-slug: organizationsorganizationid-put
  description: |-
    Updates the supplier profile of a specific organization.
    The login user must be from a supplier.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/organizationsorganizationid-put-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves the collaboration rooms of
    an organization
  x-api-slug: organizationsorganizationidcollaborationrooms-get
  description: "Retrieves the collaboration rooms where the login user's organization
    is a collaboration party.   \n- If the login user is not an organization admin,
    only the collaboration rooms where the login user is a participant are retrieved.
    \  \n- If the login user is an organization admin, all the collaboration rooms
    where the login user's organization is a collaboration party are retrieved. The
    login user may not be part of the collaborations."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/organizationsorganizationidcollaborationrooms-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves the collaboration rooms created
    by an organization
  x-api-slug: organizationsorganizationidcollaborationroomsowned-get
  description: "Retrieves the collaboration rooms created and owned by an organization.
    \ \n- If the login user is not an organization admin, only the collaboration rooms
    where the login user is a participant are retrieved.  \n- If the login user is
    an organization admin, all the collaboration rooms owned by the login user's organization
    are retrieved."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/organizationsorganizationidcollaborationroomsowned-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves a service profile
  x-api-slug: organizationsorganizationidserviceprofiles-get
  description: "Retrieves the service portfolios of a supplier.   \nA supplier may
    provide more than one type of service. The service profile may be comprised of
    various service portfolios for different service types.  \n- If the login user
    is not an organization admin, he or she can retrieve only the active service portfolios.
    \ \n- if the login user is an organization admin, he or she can retrieve both
    active and inactive service portfolios."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/organizationsorganizationidserviceprofiles-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves collaboration room template
    types
  x-api-slug: templatetypes-get
  description: Retrieves available collaboration room template types.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/templatetypes-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves the users of an organization
  x-api-slug: users-get
  description: "Retrieves the users of a specific organization.  \nThe login user
    must be from this organization as well."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/users-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves your own user info
  x-api-slug: usersself-get
  description: Retrieves the information of the current login user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/usersself-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves a user's collaboration rooms
  x-api-slug: usersuseridcollaborationrooms-get
  description: "Retrieves the collaboration rooms where a user is a participant.  \n-
    If the login user is not an organization admin, he or she can search only by his
    or her own user ID and retrieve the collaboration rooms where he or she is a participant.
    \ \n- If the login user is an organization admin, he or she can search by the
    user ID of any user in the same organization."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/usersuseridcollaborationrooms-get-openapi.md
- name: Manufacturing Network Partner APIs - Sends a callback message
  x-api-slug: callback-post
  description: |-
    Upon the receipt of an event, send a response in an async way to the event framework of Manufacturing Network.

    In the callback message, be sure to include the event ID. Add other information as appropriate.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/callback-post-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves a collaboration room
  x-api-slug: collaborationroomscollaborationroomid-get
  description: Retrieves the information of a collaboration room by its ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomid-get-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves basic info of a collaboration
    room
  x-api-slug: collaborationroomscollaborationroomidbasic-get
  description: Retrieves the information of a collaboration room in a simplified form.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidbasic-get-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves documents in a collaboration
    room
  x-api-slug: collaborationroomscollaborationroomiddocuments-get
  description: Retrieves the information of all documents in a collaboration room,
    such as design files and specifications.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomiddocuments-get-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves a document
  x-api-slug: collaborationroomscollaborationroomiddocumentsfileid-get
  description: Retrieves the information of a document by its ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomiddocumentsfileid-get-openapi.md
- name: Manufacturing Network Partner APIs - Deletes a document
  x-api-slug: collaborationroomscollaborationroomiddocumentsfileid-delete
  description: "Deletes a document.  \nThe login technical user must be the one who
    uploaded the document."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomiddocumentsfileid-delete-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves the production data
  x-api-slug: collaborationroomscollaborationroomidproductiondata-get
  description: Retrieves the production data in a collaboration room, including the
    currency, all the production options, and the initial pricings provided by the
    supplier.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/collaborationroomscollaborationroomidproductiondata-get-openapi.md
- name: Manufacturing Network Partner APIs - Downloads a file
  x-api-slug: documentscollaborationroomscollaborationroomiddownload-get
  description: Downloads a file from a collaboration room.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/documentscollaborationroomscollaborationroomiddownload-get-openapi.md
- name: Manufacturing Network Partner APIs - Uploads a file
  x-api-slug: documentscollaborationroomscollaborationroomidupload-post
  description: Uploads a file to a collaboration room.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/documentscollaborationroomscollaborationroomidupload-post-openapi.md
- name: Manufacturing Network Partner APIs - Downloads the thumbnail of a design file
  x-api-slug: documentscollaborationroomscollaborationroomidthumbnaildownload-get
  description: Downloads the thumbnail selected as the icon for a collaboration room.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/documentscollaborationroomscollaborationroomidthumbnaildownload-get-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves all extensions
  x-api-slug: extensions-get
  description: "Retrieves all the extensions that have been registered with Manufacturing
    Network.  \nThese extensions are developed by Manufacturing Network customers
    or partners to enhance the functionality of the application."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/extensions-get-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves an organization
  x-api-slug: organizationsorganizationid-get
  description: Retrieves an organization by its ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/organizationsorganizationid-get-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves the collaboration rooms of
    an organization
  x-api-slug: organizationsorganizationidcollaborationrooms-get
  description: Retrieves the collaboration rooms where an organization is a collaboration
    party.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/organizationsorganizationidcollaborationrooms-get-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves the collaboration rooms created
    by an organization
  x-api-slug: organizationsorganizationidcollaborationroomsowned-get
  description: Retrieves the collaboration rooms created and owned by an organization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/organizationsorganizationidcollaborationroomsowned-get-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves a parts analysis worklist
  x-api-slug: partsanalysisworklistsworklistid-get
  description: "Retrieves a parts analysis worklist.  \nThe analysis is made to identify
    parts that are suitable for additive manufacturing."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/partsanalysisworklistsworklistid-get-openapi.md
- name: Manufacturing Network Partner APIs - Updates a part
  x-api-slug: partsanalysisworklistsworklistidpartspartid-put
  description: Updates a part in a worklist
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/partsanalysisworklistsworklistidpartspartid-put-openapi.md
- name: Manufacturing Network Partner APIs - Downloads the design file of a part
  x-api-slug: partsanalysisworklistsworklistidpartspartiddesignfilesdesignfileid-get
  description: Downloads the design file for a part
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/partsanalysisworklistsworklistidpartspartiddesignfilesdesignfileid-get-openapi.md
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
- name: SAP Translation Hub - The '/translate' resource enables you to get translations
    of English short texts that exist in SAP Translation Hub.
  x-api-slug: translate-post
  description: Provides translations of short texts based on a combination of existing
    texts and their translations that are used in SAP products and machine translation
    capabilities.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://sandbox.api.sap.com//translationhub/api/v1
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sap/master/_listings/sap/translate-post-openapi.md
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