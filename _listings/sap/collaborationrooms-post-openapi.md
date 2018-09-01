---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Manufacturing Network Customer APIs Creates a collaboration room
  description: "Creates a collaboration room.  \nThe login user must be from a customer."
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