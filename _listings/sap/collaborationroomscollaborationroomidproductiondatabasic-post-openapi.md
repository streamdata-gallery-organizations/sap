---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Manufacturing Network Customer APIs Creates a production option without
    pricing
  description: "Creates a new production option without an initial pricing.  \nThis
    endpoint is used by users from the additive manufactuirng supplier that're not
    collaboration leads."
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
      description: "Deletes a document.  \nThe login user must be the one who uploaded
        the file."
      operationId: deletes-a-document--the-login-user-must-be-the-one-who-uploaded-the-file
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