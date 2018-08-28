---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 0
info:
  title: Pay Run.IO Gets all pay codes for specified date
  description: Gets the effective pay code revision for the specified date
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Employer/{EmployerId}/Employee/{EmployeeId}/{EffectiveDate}:
    delete:
      summary: Delete an Employee revision matching the specified revision date.
      description: Deletes the specified employee revision for the matching revision
        date
      operationId: DeleteEmployeeRevision
      x-api-path-slug: employeremployeridemployeeemployeeideffectivedate-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employee
      - Revision
      - Matching
      - Specified
      - Revision
      - Date
    get:
      summary: Get employee by effective date.
      description: Returns the employee's state at the specified effective date.
      operationId: GetEmployeeByEffectiveDate
      x-api-path-slug: employeremployeridemployeeemployeeideffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employee
      - By
      - Effective
      - Date
  /Employer/{EmployerId}/Employees/{EffectiveDate}:
    get:
      summary: Get employees from employer at a given effective date.
      description: Get links to all employees for the employer on specified effective
        date.
      operationId: GetEmployeesByEffectiveDate
      x-api-path-slug: employeremployeridemployeeseffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employees
      - From
      - Employer
      - At
      - Given
      - Effective
      - Date
  /Employer/{EmployerId}/PayCode/{PayCodeId}/{EffectiveDate}:
    get:
      summary: Gets pay code for specified date
      description: Gets the pay code revision for the specified effective date
      operationId: GetPayCodeByEffectiveDate
      x-api-path-slug: employeremployeridpaycodepaycodeideffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayCodeId
        description: The pay code unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Codespecified
      - Date
  /Employer/{EmployerId}/PayCodes/{EffectiveDate}:
    get:
      summary: Gets all pay codes for specified date
      description: Gets the effective pay code revision for the specified date
      operationId: GetPayCodesByEffectiveDate
      x-api-path-slug: employeremployeridpaycodeseffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - ""
      - Pay
      - Codesspecified
      - Date
  /Employer/{EmployerId}/Pension/{PensionId}/{EffectiveDate}:
    delete:
      summary: Delete an Pension revision matching the specified revision date.
      description: Deletes the specified pension revision for the matching revision
        date
      operationId: DeletePensionRevision
      x-api-path-slug: employeremployeridpensionpensionideffectivedate-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PensionId
        description: The pensions unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pension
      - Revision
      - Matching
      - Specified
      - Revision
      - Date
    get:
      summary: Get pension by effective date.
      description: Returns the penion's state at the specified effective date.
      operationId: GetPensionByEffectiveDate
      x-api-path-slug: employeremployeridpensionpensionideffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PensionId
        description: The pensions unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pension
      - By
      - Effective
      - Date
  /Employer/{EmployerId}/Pensions/{EffectiveDate}:
    get:
      summary: Get pensions from employer at a given effective date.
      description: Get links to all pensions for the employer on specified effective
        date.
      operationId: GetPensionsByEffectiveDate
      x-api-path-slug: employeremployeridpensionseffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pensions
      - From
      - Employer
      - At
      - Given
      - Effective
      - Date
  /Employer/{EmployerId}/{EffectiveDate}:
    delete:
      summary: Delete an Employer revision matching the specified revision date.
      description: Deletes the specified employer revision for the matching revision
        date
      operationId: DeleteEmployerRevision
      x-api-path-slug: employeremployerideffectivedate-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employer
      - Revision
      - Matching
      - Specified
      - Revision
      - Date
  /Employers/{EffectiveDate}:
    get:
      summary: Gets all employers at the specified effective date
      description: Gets links to all employers contained under the authorised application
        scope for the specified effective date.
      operationId: GetEmployersByEffectiveDate
      x-api-path-slug: employerseffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      responses:
        200:
          description: OK
      tags:
      - ""
      - Employers
      - At
      - Specified
      - Effective
      - Date
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