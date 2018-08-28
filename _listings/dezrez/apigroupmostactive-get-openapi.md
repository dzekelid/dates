---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Return the Groups with the most viewings between a given date range,
    ordered by viewing Count
  version: 1.0.0
  description: Return the groups with the most viewings between a given date range,
    ordered by viewing count.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/agency/getvatrate:
    get:
      summary: Gets the current VAT rate unless the date is specified
      description: Gets the current vat rate unless the date is specified.
      operationId: Agency_GetVatRateByvatRateTypeByvatDate
      x-api-path-slug: apiagencygetvatrate-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: vatDate
        description: Date of VAT value, used to get historic or future VAT Rates
      - in: query
        name: vatRateType
        description: Vat Rate type, standard is currently option
      responses:
        200:
          description: OK
      tags:
      - S
      - Current
      - VAT
      - Rate
      - Unless
      - Date
      - Is
      - Specified
  /api/appointment/{id}/Date/{date}:
    get:
      summary: Get details of a calculated appointment using it's id and date.
      description: Get details of a calculated appointment using it's id and date..
      operationId: Appointment_GetByidBydate
      x-api-path-slug: apiappointmentiddatedate-get
      parameters:
      - in: path
        name: date
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Details
      - Of
      - Calculated
      - Appointment
      - Using
      - Its
      - Id
      - Date
  /api/todo/updatetaskrecurrence:
    put:
      summary: Update the date of recurrence of a task
      description: Update the date of recurrence of a task.
      operationId: DefaultToDo_UpdateTaskRecurrenceBytaskRecurrence
      x-api-path-slug: apitodoupdatetaskrecurrence-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: taskRecurrence
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Recurrence
      - Of
      - Task
  /api/todo/completetask:
    put:
      summary: If Due Date is not populated a complete flag is set or if Due Date
        is populated a recurrence is set
      description: If due date is not populated a complete flag is set or if due date
        is populated a recurrence is set.
      operationId: DefaultToDo_CompleteTaskBycompleteTask
      x-api-path-slug: apitodocompletetask-put
      parameters:
      - in: body
        name: completeTask
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - If
      - Due
      - Date
      - Is
      - Not
      - Populated
      - Complete
      - Flag
      - Is
      - Set
      - If
      - Due
      - Date
      - Is
      - Populated
      - Recurrence
      - Is
      - Set
  /api/todo/event/task/duedate:
    post:
      summary: Updates the due date of an event task
      description: Updates the due date of an event task.
      operationId: EventToDo_UpdateTaskDueDateBycommandDataContract
      x-api-path-slug: apitodoeventtaskduedate-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Due
      - Date
      - Of
      - Event
      - Task
  /api/group/updateprimarygroupmember:
    put:
      summary: Return the Groups with appointments between a given date range, ordered
        by appointments Count
      description: Return the groups with appointments between a given date range,
        ordered by appointments count.
      operationId: Group_UpdatePrimaryGroupMemberByfilter
      x-api-path-slug: apigroupupdateprimarygroupmember-put
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - Groups
      - Appointments
      - Between
      - Given
      - Date
      - Range
      - ""
      - Ordered
      - By
      - Appointments
      - Count
  /api/group/mostactive:
    get:
      summary: Return the Groups with the most viewings between a given date range,
        ordered by viewing Count
      description: Return the groups with the most viewings between a given date range,
        ordered by viewing count.
      operationId: Group_MostActiveBypageSizeByfilter.rangeFromByfilter.rangeToByfilter.branchIdByfilter.roleTypes
      x-api-path-slug: apigroupmostactive-get
      parameters:
      - in: query
        name: filter.branchId
      - in: query
        name: filter.rangeFrom
      - in: query
        name: filter.rangeTo
      - in: query
        name: filter.roleTypes
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - Groups
      - Most
      - Viewings
      - Between
      - Given
      - Date
      - Range
      - ""
      - Ordered
      - By
      - Viewing
      - Count
  /api/role/{id}/setclosingdate:
    post:
      summary: Sets the role closing date
      description: Sets the role closing date.
      operationId: Role_SetClosingDateByidBydataContract
      x-api-path-slug: apiroleidsetclosingdate-post
      parameters:
      - in: body
        name: dataContract
        description: The closing data datacontract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Role
      - Closing
      - Date
  /api/progression/sales/setestimatedcompletiondate:
    put:
      summary: Set the estimated completion date on a purchasing role
      description: Set the estimated completion date on a purchasing role.
      operationId: SalesProgression_SetEstimatedCompletionDateByprogressionDateCommandDataContract
      x-api-path-slug: apiprogressionsalessetestimatedcompletiondate-put
      parameters:
      - in: body
        name: progressionDateCommandDataContract
        description: The id and datetime of the purchasing role to update the estimated
          completion date for
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Estimated
      - Completion
      - Date
      - "On"
      - Purchasing
      - Role
  /api/progression/sales/setestimatedexchangedate:
    put:
      summary: Set the estimated exchange date on a purchasing role
      description: Set the estimated exchange date on a purchasing role.
      operationId: SalesProgression_SetEstimatedExchangeDateByprogressionDateCommandDataContract
      x-api-path-slug: apiprogressionsalessetestimatedexchangedate-put
      parameters:
      - in: body
        name: progressionDateCommandDataContract
        description: The id and datetime of the purchasing role to update the estimated
          exchange date for
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Estimated
      - Exchange
      - Date
      - "On"
      - Purchasing
      - Role
  /api/tenancy/{id}/setdates:
    post:
      summary: "Set start date, terms, end date and notice period for tenancy.\r\nassertions"
      description: "Set start date, terms, end date and notice period for tenancy.\r\nassertions."
      operationId: Tenancy_SetTenancyDatesByidBydatesDataContract
      x-api-path-slug: apitenancyidsetdates-post
      parameters:
      - in: body
        name: datesDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Start
      - Date
      - ""
      - Terms
      - ""
      - End
      - Date
      - Notice
      - Periodtenancy
      - Assertions
  /api/progression/lettings/setestimatedmoveindate:
    put:
      summary: Change the estimated move in date for the tenancy.
      description: Change the estimated move in date for the tenancy..
      operationId: LettingsProgression_SetEstimatedMoveInDateBydataContract
      x-api-path-slug: apiprogressionlettingssetestimatedmoveindate-put
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Change
      - Estimated
      - Move
      - In
      - Datethe
      - Tenancy
  /api/appointment/cancel/{id}/Date/{date}:
    put:
      summary: Cancel calculated appointment by id and datetime, if it exists.
      description: Cancel calculated appointment by id and datetime, if it exists..
      operationId: Appointment_CancelByidBydateBycancelAppointmentDataContract
      x-api-path-slug: apiappointmentcanceliddatedate-put
      parameters:
      - in: body
        name: cancelAppointmentDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: date
        description: appointment start date
      - in: path
        name: id
        description: appointment id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Calculated
      - Appointment
      - By
      - Id
      - Datetime
      - ""
      - If
      - It
      - Exists
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