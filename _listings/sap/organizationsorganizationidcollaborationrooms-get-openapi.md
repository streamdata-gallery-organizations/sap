---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Manufacturing Network Partner APIs Retrieves the collaboration rooms
    of an organization
  description: Retrieves the collaboration rooms where an organization is a collaboration
    party.
  version: 1.0.0
host: hostname
basePath: /dim/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /callback:
    post:
      summary: Sends a callback message
      description: |-
        Upon the receipt of an event, send a response in an async way to the event framework of Manufacturing Network.

        In the callback message, be sure to include the event ID. Add other information as appropriate.
      operationId: upon-the-receipt-of-an-event-send-a-response-in-an-async-way-to-the-event-framework-of-manufacturing
      x-api-path-slug: callback-post
      parameters:
      - in: body
        name: Callback
        description: A callback message
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Sends
      - Callback
      - Message
  /collaborationRooms:
    post:
      summary: Creates a collaboration room
      description: "Creates a collaboration room.  \nThe login user must be from a
        customer."
      operationId: creates-a-collaboration-room--the-login-user-must-be-from-a-customer
      x-api-path-slug: collaborationrooms-post
      parameters:
      - in: body
        name: CollaborationRoomCreateRequest
        description: A request about creating a collaboration room
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - Collaboration
      - Room
  /collaborationRooms/{collaborationRoomId}:
    get:
      summary: Retrieves a collaboration room
      description: Retrieves the information of a collaboration room by its ID.
      operationId: retrieves-the-information-of-a-collaboration-room-by-its-id
      x-api-path-slug: collaborationroomscollaborationroomid-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Collaboration
      - Room
    patch:
      summary: Updates a collaboration room
      description: Updates a collaboration room.
      operationId: updates-a-collaboration-room
      x-api-path-slug: collaborationroomscollaborationroomid-patch
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: body
        name: CollaborationRoomUpdateRequest
        description: A request about updating a collaboration room
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Collaboration
      - Room
    delete:
      summary: Deletes a collaboration room
      description: |-
        Deletes a collaboration room
        The login user must be a collaboration lead for the customer and it must be a new or discarded collaboration.
      operationId: deletes-a-collaboration-roomthe-login-user-must-be-a-collaboration-lead-for-the-customer-and-it-must
      x-api-path-slug: collaborationroomscollaborationroomid-delete
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Collaboration
      - Room
  /collaborationRooms/{collaborationRoomId}/basic:
    get:
      summary: Retrieves basic info of a collaboration room
      description: Retrieves the information of a collaboration room in a simplified
        form.
      operationId: retrieves-the-information-of-a-collaboration-room-in-a-simplified-form
      x-api-path-slug: collaborationroomscollaborationroomidbasic-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Basic
      - Info
      - Of
      - Collaboration
      - Room
  /collaborationRooms/{collaborationRoomId}/start:
    post:
      summary: Starts a collaboration
      description: "Sets a collaboration in process.  \nThe collaboration must be
        a new collaboration."
      operationId: sets-a-collaboration-in-process--the-collaboration-must-be-a-new-collaboration
      x-api-path-slug: collaborationroomscollaborationroomidstart-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Starts
      - Collaboration
  /collaborationRooms/{collaborationRoomId}/complete:
    post:
      summary: Completes a collaboration
      description: |-
        Sets a collaboration as completed
        - The login user must be a collaboration lead for the customer.
        - If there's already a supplier in the collaboration room, the collaboration must already or still be in process.
        - If there's already a completed collaboration with the same additive manufacturing supplier, part ID, and customer, this operation fails.
      operationId: sets-a-collaboration-as-completed-the-login-user-must-be-a-collaboration-lead-for-the-customer-if-th
      x-api-path-slug: collaborationroomscollaborationroomidcomplete-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Completes
      - Collaboration
  /collaborationRooms/{collaborationRoomId}/discard:
    post:
      summary: Discards a collaboration
      description: "Sets a collaboration as discarded.  \nThe login user must be a
        collaboration lead for the customer and the collaboration must be in process
        or completed."
      operationId: sets-a-collaboration-as-discarded--the-login-user-must-be-a-collaboration-lead-for-the-customer-and-
      x-api-path-slug: collaborationroomscollaborationroomiddiscard-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Discards
      - Collaboration
  /collaborationRooms/{collaborationRoomId}/reopen:
    post:
      summary: Reopens a collaboration
      description: "Reopens a completed collaboration.  \nThe collaboration is set
        back to the status 'In Process'.\nThe login user must be a collaboration lead
        for the customer."
      operationId: reopens-a-completed-collaboration--the-collaboration-is-set-back-to-the-status-in-processthe-login-u
      x-api-path-slug: collaborationroomscollaborationroomidreopen-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Reopens
      - Collaboration
  /collaborationRooms/{collaborationRoomId}/documents:
    get:
      summary: Retrieves documents in a collaboration room
      description: Retrieves the information of all documents in a collaboration room,
        such as design files and specifications.
      operationId: retrieves-the-information-of-all-documents-in-a-collaboration-room-such-as-design-files-and-specific
      x-api-path-slug: collaborationroomscollaborationroomiddocuments-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Documents
      - In
      - Collaboration
      - Room
  /collaborationRooms/{collaborationRoomId}/documents/{fileId}:
    get:
      summary: Retrieves a document
      description: Retrieves the information of a document by its ID.
      operationId: retrieves-the-information-of-a-document-by-its-id
      x-api-path-slug: collaborationroomscollaborationroomiddocumentsfileid-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: path
        name: fileId
        description: The ID of a file
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Document
    delete:
      summary: Deletes a document
      description: "Deletes a document.  \nThe login technical user must be the one
        who uploaded the document."
      operationId: deletes-a-document--the-login-technical-user-must-be-the-one-who-uploaded-the-document
      x-api-path-slug: collaborationroomscollaborationroomiddocumentsfileid-delete
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: path
        name: fileId
        description: The ID of a file
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Document
  /collaborationRooms/{collaborationRoomId}/documents/{fileId}/conversion:
    get:
      summary: Gets conversion info of a design file
      description: "Retrieves the information of the conversion event for a design
        file.\nA conversion event converts a design file into a VDS file.  \nSee a
        full list of supported formats in the [online help](https://help.sap.com/viewer/dmc-mn-app-help-customer/710ee60457ca457cbda854c363bcf71f.html)."
      operationId: retrieves-the-information-of-the-conversion-event-for-a-design-filea-conversion-event-converts-a-des
      x-api-path-slug: collaborationroomscollaborationroomiddocumentsfileidconversion-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: path
        name: fileId
        description: The ID of a file
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Conversion
      - Info
      - Of
      - Design
      - File
    post:
      summary: Converts a design file
      description: |-
        Invokes a conversion event that converts a design file into a VDS file.

        See a full list of supported formats in the [online help](https://help.sap.com/viewer/dmc-mn-app-help-customer/710ee60457ca457cbda854c363bcf71f.html).
      operationId: invokes-a-conversion-event-that-converts-a-design-file-into-a-vds-filesee-a-full-list-of-supported-f
      x-api-path-slug: collaborationroomscollaborationroomiddocumentsfileidconversion-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: path
        name: fileId
        description: The ID of a file
      - in: header
        name: Prefer
        description: Sets the conversion event to run asynchronously
      responses:
        200:
          description: Successful response
      tags:
      - Converts
      - Design
      - File
  /collaborationRooms/{collaborationRoomId}/productionData:
    get:
      summary: Retrieves the production data
      description: Retrieves the production data in a collaboration room, including
        the currency, all the production options, and the initial pricings provided
        by the supplier.
      operationId: retrieves-the-production-data-in-a-collaboration-room-including-the-currency-all-the-production-opti
      x-api-path-slug: collaborationroomscollaborationroomidproductiondata-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Production
      - Data
    post:
      summary: Creates a production option
      description: "Creates a new production option, providing the pricing information
        in the meantime.  \nThe login user must be a collaboration lead from the additive
        manufacturing supplier."
      operationId: creates-a-new-production-option-providing-the-pricing-information-in-the-meantime--the-login-user-mu
      x-api-path-slug: collaborationroomscollaborationroomidproductiondata-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: body
        name: ProductionDataCreateRequest
        description: A request about creating a production option
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - Production
      - Option
  /collaborationRooms/{collaborationRoomId}/productionData/basic:
    post:
      summary: Creates a production option without pricing
      description: "Creates a new production option without an initial pricing.  \nThis
        endpoint is used by users from the additive manufactuirng supplier that're
        not collaboration leads."
      operationId: creates-a-new-production-option-without-an-initial-pricing--this-endpoint-is-used-by-users-from-the-
      x-api-path-slug: collaborationroomscollaborationroomidproductiondatabasic-post
      parameters:
      - in: body
        name: AdditionalProductionDataBasicCreateRequest
        description: A request about creating a production option without pricing
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - Production
      - Option
      - Without
      - Pricing
  /collaborationRooms/{collaborationRoomId}/productionData/original/pricing:
    put:
      summary: Updates the pricing
      description: "Updates the initial pricing for the customer's production option.
        \ \nThe login user must be a collaboration lead from an additive manufacturing
        supplier.  \nNote: The planned quantity is defined by the customer and not
        available for update by the supplier."
      operationId: updates-the-initial-pricing-for-the-customers-production-option--the-login-user-must-be-a-collaborat
      x-api-path-slug: collaborationroomscollaborationroomidproductiondataoriginalpricing-put
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: body
        name: ProductionDataPricingRequest
        description: A request about updating the pricing of a production option
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Pricing
  /collaborationRooms/{collaborationRoomId}/productionData/original/requirement:
    put:
      summary: Updates the customer's production option
      description: "Updates the customer's production option.   \nThe login user must
        be from the customer."
      operationId: updates-the-customers-production-option---the-login-user-must-be-from-the-customer
      x-api-path-slug: collaborationroomscollaborationroomidproductiondataoriginalrequirement-put
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: body
        name: ProductionDataRequirementRequest
        description: A request about a production option
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Customers
      - Production
      - Option
  /collaborationRooms/{collaborationRoomId}/productionData/{productionDataId}:
    put:
      summary: Updates a supplier's production option
      description: "Updates a production option proposed by the additive manufacturing
        supplier as well as the initial pricing for this option.  \nThe login user
        must be a collaboration lead from the additive manufacturing supplier."
      operationId: updates-a-production-option-proposed-by-the-additive-manufacturing-supplier-as-well-as-the-initial-p
      x-api-path-slug: collaborationroomscollaborationroomidproductiondataproductiondataid-put
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: path
        name: productionDataId
        description: The ID of a production option
      - in: body
        name: ProductionDataUpdateRequest
        description: A request about updating a production option
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Suppliers
      - Production
      - Option
    delete:
      summary: Deletes a supplier's production option
      description: "Deletes a production option proposed by the additive manufacturing
        supplier. The initial pricing is deleted along with it.  \nThe login user
        must be from the additive manufacturing supplier."
      operationId: deletes-a-production-option-proposed-by-the-additive-manufacturing-supplier-the-initial-pricing-is-d
      x-api-path-slug: collaborationroomscollaborationroomidproductiondataproductiondataid-delete
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: path
        name: productionDataId
        description: The ID of a production option
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Suppliers
      - Production
      - Option
  /collaborationRooms/{collaborationRoomId}/productionData/{productionDataId}/basic:
    put:
      summary: Updates a supplier's production option
      description: "Updates a production option proposed by the additive manufacturing
        supplier.    \nThis endpoint is used by users from the additive manufactuirng
        supplier that're not collaboration leads. The initial pricing cannot be updated."
      operationId: updates-a-production-option-proposed-by-the-additive-manufacturing-supplier----this-endpoint-is-used
      x-api-path-slug: collaborationroomscollaborationroomidproductiondataproductiondataidbasic-put
      parameters:
      - in: body
        name: AdditionalProductionDataBasicUpdateRequest
        description: A request about updating a suppliers production option, excluding
          pricing information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: path
        name: productionDataId
        description: The ID of a production option
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Suppliers
      - Production
      - Option
  /collaborationRooms/{collaborationRoomId}/productionData/confirmed:
    get:
      summary: Retrieves the confirmed production option
      description: Retrieves the production option confirmed as the finalized production
        requirements, and the initial pricing for it.
      operationId: retrieves-the-production-option-confirmed-as-the-finalized-production-requirements-and-the-initial-p
      x-api-path-slug: collaborationroomscollaborationroomidproductiondataconfirmed-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Confirmed
      - Production
      - Option
  /collaborationRooms/{collaborationRoomId}/productionData/{productionDataId}/confirm:
    post:
      summary: Confirms a production option
      description: "Confirms a production option along with the initial pricing for
        it.  \nThe production option might be proposed by the customer or the additive
        manufacturing supplier.   \nThe login user must be from the customer."
      operationId: confirms-a-production-option-along-with-the-initial-pricing-for-it--the-production-option-might-be-p
      x-api-path-slug: collaborationroomscollaborationroomidproductiondataproductiondataidconfirm-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: path
        name: productionDataId
        description: The ID of a production option
      responses:
        200:
          description: Successful response
      tags:
      - Confirms
      - Production
      - Option
  /collaborationRooms/{collaborationRoomId}/productionData/{productionDataId}/cancelConfirm:
    post:
      summary: Cancels the confirmation of a production option
      description: "Undos the confirmation of a production option.  \nThe login user
        must be from the customer."
      operationId: undos-the-confirmation-of-a-production-option--the-login-user-must-be-from-the-customer
      x-api-path-slug: collaborationroomscollaborationroomidproductiondataproductiondataidcancelconfirm-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: path
        name: productionDataId
        description: The ID of a production option
      responses:
        200:
          description: Successful response
      tags:
      - Cancels
      - Confirmation
      - Of
      - Production
      - Option
  /collaborationRooms/{collaborationRoomId}/thumbnails:
    get:
      summary: Retrieves the thumbnail of a design file
      description: |-
        Retrieves the thumbnail information in a collaboration room.
        Each design file has a corresponding thumbnail file automatically generated.
      operationId: retrieves-the-thumbnail-information-in-a-collaboration-roomeach-design-file-has-a-corresponding-thum
      x-api-path-slug: collaborationroomscollaborationroomidthumbnails-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Thumbnail
      - Of
      - Design
      - File
  /collaborationTemplates:
    get:
      summary: Retrieves available collaboration room templates
      description: Retrieves available collaboration room templates.
      operationId: retrieves-available-collaboration-room-templates
      x-api-path-slug: collaborationtemplates-get
      parameters:
      - in: query
        name: typeId
        description: The ID of a collaboration room template
      - in: query
        name: typeName
        description: The name of a collaboration room template
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Available
      - Collaboration
      - Room
      - Templates
  /documents/collaborationRooms/{collaborationRoomId}/download:
    get:
      summary: Downloads a file
      description: Downloads a file from a collaboration room.
      operationId: downloads-a-file-from-a-collaboration-room
      x-api-path-slug: documentscollaborationroomscollaborationroomiddownload-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: query
        name: fileId
        description: The ID of a file
      responses:
        200:
          description: Successful response
      tags:
      - Downloads
      - File
  /documents/collaborationRooms/{collaborationRoomId}/upload:
    post:
      summary: Uploads a file
      description: Uploads a file to a collaboration room.
      operationId: uploads-a-file-to-a-collaboration-room
      x-api-path-slug: documentscollaborationroomscollaborationroomidupload-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: formData
        name: fileUpload
        description: A file to be uploaded
      - in: formData
        name: originFileDisplay
        description: Indicates if a file is visible to all participants in the collaboration
          room (public) or to the uploader only (private)
      responses:
        200:
          description: Successful response
      tags:
      - Uploads
      - File
  /documents/collaborationRooms/{collaborationRoomId}/thumbnail/download:
    get:
      summary: Downloads the thumbnail of a design file
      description: Downloads the thumbnail selected as the icon for a collaboration
        room.
      operationId: downloads-the-thumbnail-selected-as-the-icon-for-a-collaboration-room
      x-api-path-slug: documentscollaborationroomscollaborationroomidthumbnaildownload-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Downloads
      - Thumbnail
      - Of
      - Design
      - File
  /documents/organizations/{organizationId}/TEMP/upload:
    post:
      summary: Uploads a file to the temp folder
      description: Uploads a file to the temp folder for an organization.
      operationId: uploads-a-file-to-the-temp-folder-for-an-organization
      x-api-path-slug: documentsorganizationsorganizationidtempupload-post
      parameters:
      - in: formData
        name: fileUpload
        description: A file to be uploaded
      - in: path
        name: organizationId
        description: The ID of an organization
      responses:
        200:
          description: Successful response
      tags:
      - Uploads
      - File
      - To
      - Temp
      - Folder
  /extensions:
    get:
      summary: Retrieves all extensions
      description: "Retrieves all the extensions that have been registered with Manufacturing
        Network.  \nThese extensions are developed by Manufacturing Network customers
        or partners to enhance the functionality of the application."
      operationId: retrieves-all-the-extensions-that-have-been-registered-with-manufacturing-network--these-extensions-
      x-api-path-slug: extensions-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - ""
      - Extensions
  /extensions/available:
    get:
      summary: Retrieves extensions available for use
      description: "Retrieves extensions that can be used during a collaboration.
        \ \nA supplier enables an extension for collaboration by selecting it for
        use in the supplier profile."
      operationId: retrieves-extensions-that-can-be-used-during-a-collaboration--a-supplier-enables-an-extension-for-co
      x-api-path-slug: extensionsavailable-get
      parameters:
      - in: query
        name: organizationIds
        description: The IDs of organizations as collaboration partiesSeparate the
          IDs using commas
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Extensions
      - Availableuse
  /masterData:
    get:
      summary: Retrieves supplier profile master data
      description: |-
        Retrieves master data such as processes and materials.
        Narrow down the result by specifying the master data types.
      operationId: retrieves-master-data-such-as-processes-and-materialsnarrow-down-the-result-by-specifying-the-master
      x-api-path-slug: masterdata-get
      parameters:
      - in: query
        name: type
        description: 'A master data typeValid values: [certificates, currencies, materialRequirement,
          postProcesses, preferredLanguages, processMaterial, servicePortfolio]'
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Supplier
      - Profile
      - Master
      - Data
  /orders:
    post:
      summary: Creates an order
      description: |-
        Creates an order for the part for which the customer and the supplier haven been colloabrating
        The order is based on the confirmed production option and pricing.
        The login user must be from the customer.
      operationId: creates-an-order-for-the-part-for-which-the-customer-and-the-supplier-haven-been-colloabratingthe-or
      x-api-path-slug: orders-post
      parameters:
      - in: body
        name: OrderRequest
        description: A request about an order
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - Order
  /orders/{orderNumber}/history:
    post:
      summary: Adds a record to the order history
      description: "Adds a record to the history of an order.   \nThe order number
        is sent in the message body of the Order Created event.  \nThe login user
        must be from the additive manufacturing supplier."
      operationId: adds-a-record-to-the-history-of-an-order---the-order-number-is-sent-in-the-message-body-of-the-order
      x-api-path-slug: ordersordernumberhistory-post
      parameters:
      - in: body
        name: OrderItemRequest
        description: A request about an order
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderNumber
        description: An order number
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Record
      - To
      - Order
      - History
  /organizations/self:
    get:
      summary: Retrieves your own organization
      description: Retrieves the information of the login user's own organization.
      operationId: retrieves-the-information-of-the-login-users-own-organization
      x-api-path-slug: organizationsself-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Your
      - Own
      - Organization
  /organizations/visible:
    get:
      summary: Retrieves organizations available for collaboration
      description: "Retrieves organizations in a specific business role that are available
        for collaboration.  \nThese organizations may have been approved for or blocked
        from collaboration, or they're still pending for approval.\nThe login user
        must be from a customer."
      operationId: retrieves-organizations-in-a-specific-business-role-that-are-available-for-collaboration--these-orga
      x-api-path-slug: organizationsvisible-get
      parameters:
      - in: query
        name: activeServices
        description: The types of service that a supplier provides
      - in: query
        name: approved
        description: Specify approved=true to restrict the search to organizations
          that are approved for collaboration
      - in: query
        name: roleCode
        description: The code for the business role of the organizations
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Organizations
      - Availablecollaboration
  /organizations/{organizationId}:
    get:
      summary: Retrieves an organization
      description: Retrieves an organization by its ID.
      operationId: retrieves-an-organization-by-its-id
      x-api-path-slug: organizationsorganizationid-get
      parameters:
      - in: path
        name: organizationId
        description: The ID of an organization
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Organization
    put:
      summary: Updates a supplier profile
      description: |-
        Updates the supplier profile of a specific organization.
        The login user must be from a supplier.
      operationId: updates-the-supplier-profile-of-a-specific-organizationthe-login-user-must-be-from-a-supplier
      x-api-path-slug: organizationsorganizationid-put
      parameters:
      - in: path
        name: organizationId
        description: The ID of the login users organization
      - in: body
        name: OrganizationUpdateRequest
        description: A request about updating an organization
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Supplier
      - Profile
  /organizations/{organizationId}/collaborationRooms:
    get:
      summary: Retrieves the collaboration rooms of an organization
      description: Retrieves the collaboration rooms where an organization is a collaboration
        party.
      operationId: retrieves-the-collaboration-rooms-where-an-organization-is-a-collaboration-party---
      x-api-path-slug: organizationsorganizationidcollaborationrooms-get
      parameters:
      - in: path
        name: organizationId
        description: The ID of an organization
      - in: query
        name: organizationIds
        description: The IDs of other organizations
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Collaboration
      - Rooms
      - Of
      - Organization
  /organizations/{organizationId}/collaborationRooms/owned:
    get:
      summary: Retrieves the collaboration rooms created by an organization
      description: "Retrieves the collaboration rooms created and owned by an organization.
        \ \n- If the login user is not an organization admin, only the collaboration
        rooms where the login user is a participant are retrieved.  \n- If the login
        user is an organization admin, all the collaboration rooms owned by the login
        user's organization are retrieved."
      operationId: retrieves-the-collaboration-rooms-created-and-owned-by-an-organization---if-the-login-user-is-not-an
      x-api-path-slug: organizationsorganizationidcollaborationroomsowned-get
      parameters:
      - in: path
        name: organizationId
        description: The ID of the login users organization
      - in: query
        name: organizationIds
        description: The IDs of other organizations
      - in: query
        name: partId
        description: The ID of a part
      - in: query
        name: serviceType
        description: The type of service that a supplier organization provides during
          the collaboration
      - in: query
        name: status
        description: The status of a collaboration
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Collaboration
      - Rooms
      - Created
      - By
      - Organization
  /organizations/{organizationId}/serviceProfiles:
    get:
      summary: Retrieves a service profile
      description: "Retrieves the service portfolios of a supplier.   \nA supplier
        may provide more than one type of service. The service profile may be comprised
        of various service portfolios for different service types.  \n- If the login
        user is not an organization admin, he or she can retrieve only the active
        service portfolios.  \n- if the login user is an organization admin, he or
        she can retrieve both active and inactive service portfolios."
      operationId: retrieves-the-service-portfolios-of-a-supplier---a-supplier-may-provide-more-than-one-type-of-servic
      x-api-path-slug: organizationsorganizationidserviceprofiles-get
      parameters:
      - in: path
        name: organizationId
        description: The ID of the login users organization
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Service
      - Profile
  /templateTypes:
    get:
      summary: Retrieves collaboration room template types
      description: Retrieves available collaboration room template types.
      operationId: retrieves-available-collaboration-room-template-types
      x-api-path-slug: templatetypes-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Collaboration
      - Room
      - Template
      - Types
  /users:
    get:
      summary: Retrieves the users of an organization
      description: "Retrieves the users of a specific organization.  \nThe login user
        must be from this organization as well."
      operationId: retrieves-the-users-of-a-specific-organization--the-login-user-must-be-from-this-organization-as-wel
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: organizationId
        description: The ID of an organization
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Users
      - Of
      - Organization
  /users/self:
    get:
      summary: Retrieves your own user info
      description: Retrieves the information of the current login user.
      operationId: retrieves-the-information-of-the-current-login-user
      x-api-path-slug: usersself-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Your
      - Own
      - User
      - Info
  /users/{userId}/collaborationRooms:
    get:
      summary: Retrieves a user's collaboration rooms
      description: "Retrieves the collaboration rooms where a user is a participant.
        \ \n- If the login user is not an organization admin, he or she can search
        only by his or her own user ID and retrieve the collaboration rooms where
        he or she is a participant.  \n- If the login user is an organization admin,
        he or she can search by the user ID of any user in the same organization."
      operationId: retrieves-the-collaboration-rooms-where-a-user-is-a-participant---if-the-login-user-is-not-an-organi
      x-api-path-slug: usersuseridcollaborationrooms-get
      parameters:
      - in: path
        name: userId
        description: The ID of a user
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Users
      - Collaboration
      - Rooms
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