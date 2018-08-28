swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/gradebook_history/date:
    get:
      summary: Details for a given date in gradebook history for this course
      description: Details for a given date in gradebook history for this course.
      operationId: details-for-a-given-date-in-gradebook-history-for-this-course
      x-api-path-slug: coursescourse-idgradebook-historydate-get
      parameters:
      - in: query
        name: course_id
        description: The id of the contextual course for this API call
      - in: query
        name: date
        description: The date for which you would like to see detailed information
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Gradebook
      - History
      - Date
  /courses/{course_id}/gradebook_history/date/graders/{grader_id}/assignments/assignment_id/submissions:
    get:
      summary: Lists submissions
      description: Lists submissions.
      operationId: lists-submissions
      x-api-path-slug: coursescourse-idgradebook-historydategradersgrader-idassignmentsassignment-idsubmissions-get
      parameters:
      - in: query
        name: assignment_id
        description: The ID of the assignment for which you want to see submissions
      - in: query
        name: course_id
        description: The id of the contextual course for this API call
      - in: query
        name: date
        description: The date for which you would like to see submissions
      - in: query
        name: grader_id
        description: The ID of the grader for which you want to see submissions
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Gradebook
      - History
      - Date
      - Graders
      - Grader
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions