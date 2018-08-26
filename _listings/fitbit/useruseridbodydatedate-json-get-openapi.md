---
swagger: "2.0"
x-collection-name: Fitbit
x-complete: 0
info:
  title: Fitbit Get User User Body Date Date .json
  description: Get a summary of a user's body measurements for a given day in the
    format requested using units in the unit system which corresponds to the Accept-Language
    header provided.
  version: 1.0.0
host: api.fitbit.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/-/foods/log/water/date/{date}.json:
    get:
      summary: Get User Foods Log Water Date Date .json
      description: Get a summary and list of a user's water log entries for a given
        day in the format requested using units in the unit system which corresponds
        to the Accept-Language header provided.
      operationId: getUserFoodsLogWaterDateDate.json
      x-api-path-slug: userfoodslogwaterdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Water
      - Date
      - Date.json
  /user/{user-id}/sleep/minutesAsleep/date/{start-date-or-end-date}/{end-date-or-period}.json:
    get:
      summary: Get User User Sleep Minutesasleep Date Start Date Or End Date End Date
        Or Period .json
      description: Get time series in the specified range for a given resource in
        the format requested using units in the unit system which corresponds to the
        Accept-Language header provided.
      operationId: getUserUserSleepMinutesasleepDateStartDateOrEndDateEndDateOrPeriod.json
      x-api-path-slug: useruseridsleepminutesasleepdatestartdateorenddateenddateorperiod-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Sleep
      - MinutesAsleep
      - Date
      - Start-date-or-end-date
      - End-date-or-period.json
  /user/{user-id}/foods/log/caloriesIn/date/{start-date-or-end-date}/{end-date-or-period}.json:
    get:
      summary: Get User User Foods Log Caloriesin Date Start Date Or End Date End
        Date Or Period .json
      description: Get time series in the specified range for a given resource in
        the format requested using units in the unit system which corresponds to the
        Accept-Language header provided.
      operationId: getUserUserFoodsLogCaloriesinDateStartDateOrEndDateEndDateOrPeriod.json
      x-api-path-slug: useruseridfoodslogcaloriesindatestartdateorenddateenddateorperiod-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Foods
      - Log
      - CaloriesIn
      - Date
      - Start-date-or-end-date
      - End-date-or-period.json
  /user/{user-id}/body/weight/date/{start-date-or-end-date}/{end-date-or-period}.json:
    get:
      summary: Get User User Body Weight Date Start Date Or End Date End Date Or Period
        .json
      description: Get time series in the specified range for a given resource in
        the format requested using units in the unit system which corresponds to the
        Accept-Language header provided.
      operationId: getUserUserBodyWeightDateStartDateOrEndDateEndDateOrPeriod.json
      x-api-path-slug: useruseridbodyweightdatestartdateorenddateenddateorperiod-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Body
      - Weight
      - Date
      - Start-date-or-end-date
      - End-date-or-period.json
  /user/{user-id}/activities/calories/date/{start-date-or-end-date}/{end-date-or-period}.json:
    get:
      summary: Get User User Activities Calories Date Start Date Or End Date End Date
        Or Period .json
      description: Get time series in the specified range for a given resource in
        the format requested using units in the unit system which corresponds to the
        Accept-Language header provided.
      operationId: getUserUserActivitiesCaloriesDateStartDateOrEndDateEndDateOrPeriod.json
      x-api-path-slug: useruseridactivitiescaloriesdatestartdateorenddateenddateorperiod-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Activities
      - Calories
      - Date
      - Start-date-or-end-date
      - End-date-or-period.json
  /user/-/glucose/date/{date}.json:
    get:
      summary: Get User Glucose Date Date .json
      description: Get a list of user's blood glucose and HbA1C measurements for a
        given day in the format requested using units in the unit system which corresponds
        to the Accept-Language header provided. Glucose measurement log entries are
        available only to authorized user. We always include all glucose trackers
        in the response body (with zero glucose value for the days with no measurements)
        to allow to seamlessly fetch a list of all additional user created custom
        trackers.
      operationId: getUserGlucoseDateDate.json
      x-api-path-slug: userglucosedatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Glucose
      - Date
      - Date.json
  /user/-/bp/date/{date}.json:
    get:
      summary: Get User Bp Date Date .json
      description: Get an average value and a list of user's blood pressure log entries
        for a given day in the format requested. Blood pressure log entries are available
        only to authorized user. Blood pressure log entries in response are sorted
        exactly the same as they are presented on the Fitbit website.
      operationId: getUserBpDateDate.json
      x-api-path-slug: userbpdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Bp
      - Date
      - Date.json
  /user/-/heart/date/{date}.json:
    get:
      summary: Get User Heart Date Date .json
      description: Get an average values and a list of user's heart rate log entries
        for a given day in the format requested. Heart rate data available only to
        the authorized user. Heart rate log entries in response are sorted exactly
        the same as they are presented on the Fitbit website. We always include all
        heart rate trackers in the "average" section of the response body (with zero
        average values for the days with no measurements) to allow to seamlessly fetch
        a list of all additional user created custom trackers.
      operationId: getUserHeartDateDate.json
      x-api-path-slug: userheartdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Heart
      - Date
      - Date.json
  /user/{user-id}/sleep/date/{date}.json:
    get:
      summary: Get User User Sleep Date Date .json
      description: Get a summary and list of a user's sleep log entries for a given
        day in the format requested. Endpoint returns summary for all sleep log entries
        for the given day (including naps). If you need data only for the main sleep
        you can fetch entry with "isMainSleep" = true or use Get-Time-Series calls.
      operationId: getUserUserSleepDateDate.json
      x-api-path-slug: useruseridsleepdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Sleep
      - Date
      - Date.json
  /user/{user-id}/foods/log/date/{date}.json:
    get:
      summary: Get User User Foods Log Date Date .json
      description: Get a summary and list of a user's food log entries for a given
        day in the format requested.
      operationId: getUserUserFoodsLogDateDate.json
      x-api-path-slug: useruseridfoodslogdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Foods
      - Log
      - Date
      - Date.json
  /user/{user-id}/activities/date/{date}.json:
    get:
      summary: Get User User Activities Date Date .json
      description: Get a summary and list of a user's activities and activity log
        entries for a given day in the format requested using units in the unit system
        which corresponds to the Accept-Language header provided.
      operationId: getUserUserActivitiesDateDate.json
      x-api-path-slug: useruseridactivitiesdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Activities
      - Date
      - Date.json
  /user/-/body/log/fat/date/{date}.json:
    get:
      summary: Get User Body Log Fat Date Date .json
      description: Get a list of all user's body fat log entries for a given day in
        the format requested.
      operationId: getUserBodyLogFatDateDate.json
      x-api-path-slug: userbodylogfatdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body
      - Log
      - Fat
      - Date
      - Date.json
  /user/-/body/log/weight/date/{date}.json:
    get:
      summary: Get User Body Log Weight Date Date .json
      description: Get a list of all user's body weight log entries for a given day
        in the format requested using units in the unit system which corresponds to
        the Accept-Language header provided.
      operationId: getUserBodyLogWeightDateDate.json
      x-api-path-slug: userbodylogweightdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body
      - Log
      - Weight
      - Date
      - Date.json
  /user/{user-id}/body/date/{date}.json:
    get:
      summary: Get User User Body Date Date .json
      description: Get a summary of a user's body measurements for a given day in
        the format requested using units in the unit system which corresponds to the
        Accept-Language header provided.
      operationId: getUserUserBodyDateDate.json
      x-api-path-slug: useruseridbodydatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Body
      - Date
      - Date.json
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