{
  "info": {
    "name": "Fitbit Get User Glucose Date Date .json",
    "_postman_id": "bb7907f7-cf03-42e3-9de2-762ec4e0e855",
    "description": "Get a list of user's blood glucose and HbA1C measurements for a given day in the format requested using units in the unit system which corresponds to the Accept-Language header provided. Glucose measurement log entries are available only to authorized user. We always include all glucose trackers in the response body (with zero glucose value for the days with no measurements) to allow to seamlessly fetch a list of all additional user created custom trackers.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "1f6ca6ed-87ab-488a-b381-05449f909571",
          "name": "getUserCollectionPathApisubscriptions.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-:collection-pathapiSubscriptions.json"
              ],
              "variable": [
                {
                  "id": "collection-path",
                  "value": "collection-path",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of user's subscriptions for your application in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3ae631d-5abb-4883-ade4-d1f28c393c83"
            }
          ]
        },
        {
          "id": "19363bf0-c70d-49df-bc8f-41be26d20ae9",
          "name": "postUserCollectionPathApisubscriptionsSubscription.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-:collection-pathapiSubscriptions/:subscription-id.json"
              ],
              "variable": [
                {
                  "id": "collection-path",
                  "value": "collection-path",
                  "type": "string"
                },
                {
                  "id": "subscription-id",
                  "value": "subscription-id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a subscription for the user to get notifications and get a response in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf5903f7-5f81-4749-8b6c-7a786c586b06"
            }
          ]
        },
        {
          "id": "52a2b0a6-858e-4c2b-b855-24613efd97b8",
          "name": "deleteUserCollectionPathApisubscriptionsSubscription.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-:collection-pathapiSubscriptions/:subscription-id.json"
              ],
              "variable": [
                {
                  "id": "collection-path",
                  "value": "collection-path",
                  "type": "string"
                },
                {
                  "id": "subscription-id",
                  "value": "subscription-id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a subscription for the user and get a response in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eed35196-9f3f-496f-a8a4-9eb1a4f224ea"
            }
          ]
        },
        {
          "id": "36f6a0b2-8be7-412f-b4c2-32899b56cf5b",
          "name": "getUserFriendsInvitations.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/friends/invitations.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the list of invites to become freinds for a user in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c731ba2-597a-4442-8ab8-3c4b7efce944"
            }
          ]
        },
        {
          "id": "068af00c-3fdc-40b2-b88a-12e9c480581c",
          "name": "getUserDevices.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/devices.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the list of Fitbit devices for a user in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4dbe51e8-e195-40d2-a0d2-8151d7d8f12e"
            }
          ]
        },
        {
          "id": "b03149b6-c452-4025-a6f1-94e164000a66",
          "name": "getUserFoodsLogGoal.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/foods/log/goal.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a user's current daily calorie consumption goal and/or Food Plan in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30842645-7ee5-4676-ac03-516d42b4fcc8"
            }
          ]
        },
        {
          "id": "9468ca06-825f-4b77-9042-8cefc539cc0b",
          "name": "postUserFoodsLogGoal.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/foods/log/goal.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Update (create) a user's daily calorie consumption goal or Food Plan and get a response in the format requested. Food Plan could not be created unless user already has active goal (Update-Weight-Goal). Depending on the weight goal setup only either MAINTENANCE (in case start weight is close to target weight or smaller) or one of the four other \"lose\" food plans could be created via intensity POST parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c52b1b0-69b7-4321-9278-23220377c98f"
            }
          ]
        },
        {
          "id": "7302c0cf-1a69-4dd4-b544-febb080c7548",
          "name": "getUserMeals.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/meals.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of meals user created in his food log in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55696057-158d-44e8-94f4-272023f3aec1"
            }
          ]
        },
        {
          "id": "5dae36da-d5b7-4959-b969-1b76af8bf1c5",
          "name": "deleteUserFoodsLogWaterWaterLog.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/foods/log/water/:water-log-id.json"
              ],
              "variable": [
                {
                  "id": "water-log-id",
                  "value": "water-log-id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete user's water log entry with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66e44340-a010-4f48-ba1b-963e87fb864b"
            }
          ]
        },
        {
          "id": "056bda0e-f9ef-4096-b455-f56599b504f2",
          "name": "postUserFoodsLogWater.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/foods/log/water.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create log entry for a water using units in the unit system that corresponds to the Accept-Language header provided (or waterUnit) and get a response in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4cc75330-7301-48ee-a9af-6e6603e07098"
            }
          ]
        },
        {
          "id": "8af86fc6-8af6-4ef4-ba16-b0162aa29859",
          "name": "getUserFoodsLogWaterDateDate.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/foods/log/water/date/:date.json"
              ],
              "variable": [
                {
                  "id": "date",
                  "value": "date",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a summary and list of a user's water log entries for a given day in the format requested using units in the unit system which corresponds to the Accept-Language header provided."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec14d08f-90e4-41b2-aa2f-8ddff7f9c306"
            }
          ]
        },
        {
          "id": "c910edad-cc06-455b-a082-84944e0170f8",
          "name": "postUserFoodsLogFavorite.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/foods/log/favorite/:id.json"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add the food with the given id to user's list of favorite foods."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fab9284-560b-446d-be47-2a59fe24ab73"
            }
          ]
        },
        {
          "id": "eae620d3-3cf6-41a1-9b85-5dae1276917e",
          "name": "deleteUserFoodsLogFavorite.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/foods/log/favorite/:id.json"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete the food with the given id from user's list of favorite foods."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa7f8d51-8939-401a-b57f-1d23c741fab1"
            }
          ]
        },
        {
          "id": "6ca4d696-02fd-43db-8b69-c5d2722b9ce4",
          "name": "getUserActivitiesGoalsWeekly.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/activities/goals/weekly.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a user's current weekly activity goals in the format requested using units in the unit system which corresponds to the Accept-Language header provided."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5de3e3e5-770d-4e91-8591-dbe232c6879e"
            }
          ]
        },
        {
          "id": "ab0ff497-796f-4083-8cd4-869ed7ac8eb5",
          "name": "getUserActivitiesGoalsDaily.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/activities/goals/daily.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a user's current daily activity goals in the format requested using units in the unit system which corresponds to the Accept-Language header provided."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0a8a800-0071-49a2-8d73-7f75fea0f0d9"
            }
          ]
        },
        {
          "id": "1e1ddd68-eaa5-44f8-92fb-e175661e51b6",
          "name": "postUserActivitiesLogFavorite.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/activities/log/favorite/:id.json"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the activity with the given id to user's list of favorite activities."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63813baf-a931-471c-8448-b18f7960e2de"
            }
          ]
        },
        {
          "id": "e5b5621e-3331-4722-930e-a203eb3bcc82",
          "name": "deleteUserActivitiesLogFavorite.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/activities/log/favorite/:id.json"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete the activity with the given id from user's list of favorite activities."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f5f94ef-df76-4f77-89af-d155ed5febe2"
            }
          ]
        },
        {
          "id": "7434de61-b2d8-4bab-bb98-ddd0be1a393f",
          "name": "getUserFoodsLogFavorite.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/foods/log/favorite.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of a user's favorite foods in the format requested. A user marks a food as favorite on the user's Food Tab tab. A favorite food in the list provides a quick way to log the food via the Log Food endpoint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2fe8a27e-e7b7-4536-bf1f-1559164247f6"
            }
          ]
        },
        {
          "id": "02c4b2e9-1d88-4c88-bd4e-8a72d73663cb",
          "name": "getUserFoodsLogFrequent.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/foods/log/frequent.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of a user's frequent foods in the format requested. A frequent food in the list provides a quick way to log the food via the Log Food endpoint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f43053d-9ae9-4230-8228-54019bc8cf37"
            }
          ]
        },
        {
          "id": "a2fac29f-6e64-48a3-82a7-0e38ecfe1739",
          "name": "getUserFoodsLogRecent.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/foods/log/recent.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of a user's recent foods in the format requested. A recent food provides a quick way to log the food via the Log Food endpoint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ab11ba5-e522-49e4-834a-8cd1cf2aa651"
            }
          ]
        },
        {
          "id": "da1cdb25-2963-4642-9229-079de0c2ddbb",
          "name": "getUserActivitiesFavorite.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/activities/favorite.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of a user's favorite activities in the format requested. A user marks an activity as favorite on the user's Activities Tab. The activity ids in the list can be used to create a new activity log entry via the Log Activity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58a5ad3f-4988-4f22-aa49-75d5f2a0dee4"
            }
          ]
        },
        {
          "id": "71d2f7a9-a493-466b-a4b0-c0b44e3b917a",
          "name": "getUserActivitiesFrequent.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/activities/frequent.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of a user's frequent activities in the format requested using units in the unit system which corresponds to the Accept-Language header provided. A frequent activity record contains the distance and duration values recorded the last time the activity was logged. The record retrieved can therefore be used to log the activity via the Log Activity with the same or adjusted values for distance and duration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a01d24c-023d-4434-b52f-c7847e58ed96"
            }
          ]
        },
        {
          "id": "979645bc-fc60-4942-87b5-99f424bdb90b",
          "name": "getUserActivitiesRecent.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/activities/recent.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of a user's recent activities in the format requested using units in the unit system which corresponds to the Accept-Language header provided. A recent activity record contains the distance and duration values recorded the last time the activity was logged. The record retrieved can therefore be used to log the activity via the Log Activity with the same or adjusted values for distance and duration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74f69f06-954a-4f04-8e51-2d446407fad4"
            }
          ]
        },
        {
          "id": "e8c701d9-a206-4bb4-a061-f88c7d06f56c",
          "name": "getUserUserSleepMinutesasleepDateStartDateOrEndDateEndDateOrPeriod.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/:user-id/sleep/minutesAsleep/date/:start-date-or-end-date/:end-date-or-period.json"
              ],
              "variable": [
                {
                  "id": "user-id",
                  "value": "user-id",
                  "type": "string"
                },
                {
                  "id": "start-date-or-end-date",
                  "value": "start-date-or-end-date",
                  "type": "string"
                },
                {
                  "id": "end-date-or-period",
                  "value": "end-date-or-period",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get time series in the specified range for a given resource in the format requested using units in the unit system which corresponds to the Accept-Language header provided."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ccb8f1a-8b0d-4b69-849d-9b231ff1ce2d"
            }
          ]
        },
        {
          "id": "e4393723-891f-48a3-81f6-ba257ac876e4",
          "name": "getUserUserFoodsLogCaloriesinDateStartDateOrEndDateEndDateOrPeriod.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/:user-id/foods/log/caloriesIn/date/:start-date-or-end-date/:end-date-or-period.json"
              ],
              "variable": [
                {
                  "id": "user-id",
                  "value": "user-id",
                  "type": "string"
                },
                {
                  "id": "start-date-or-end-date",
                  "value": "start-date-or-end-date",
                  "type": "string"
                },
                {
                  "id": "end-date-or-period",
                  "value": "end-date-or-period",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get time series in the specified range for a given resource in the format requested using units in the unit system which corresponds to the Accept-Language header provided."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "117d6599-5a5f-446d-bd71-9857186bbb1d"
            }
          ]
        },
        {
          "id": "165c9b1b-9a32-44ce-9b59-f238204beb3f",
          "name": "getUserBodyLogFatGoal.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/body/log/fat/goal.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a user's current fat goal in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f1af3cd-c222-4266-bcab-ec5196b1b55f"
            }
          ]
        },
        {
          "id": "22c2b11a-4eb1-4f51-86a5-b059d52c5d35",
          "name": "postUserBodyLogFatGoal.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/body/log/fat/goal.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create or updates user's fat goal and get a response in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f89d79f-bac6-4818-9e34-1e65225a2a54"
            }
          ]
        },
        {
          "id": "e70152e4-0014-469e-85e8-e88b69ee8397",
          "name": "getUserBodyLogWeightGoal.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/body/log/weight/goal.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a user's current weight goal using units in the unit system that corresponds to the Accept-Language header provided in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f0e4edb-3193-4e24-a928-91baf1b0ed74"
            }
          ]
        },
        {
          "id": "5ad56c56-3284-467c-83b6-8e8e80f94cdb",
          "name": "postUserBodyLogWeightGoal.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/body/log/weight/goal.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create or update user's weight goal using units in the unit system that corresponds to the Accept-Language header provided and get a response in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57d281ce-5cd7-48f9-b058-69fb88a0b3ce"
            }
          ]
        },
        {
          "id": "3eb3545e-22b8-4666-9be2-5900f7977eae",
          "name": "deleteUserBodyLogFatBodyFatLog.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/body/log/fat/:body-fat-log-id.json"
              ],
              "variable": [
                {
                  "id": "body-fat-log-id",
                  "value": "body-fat-log-id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete user's body fat log entry with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01337129-a3e5-4995-9887-086fb4f1afc3"
            }
          ]
        },
        {
          "id": "747f89a3-cc75-40fc-bfc0-b9780c52d11a",
          "name": "deleteUserBodyLogFatBodyWeightLog.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/body/log/fat/:body-weight-log-id.json"
              ],
              "variable": [
                {
                  "id": "body-weight-log-id",
                  "value": "body-weight-log-id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete user's body weight log entry with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58005bd2-395f-4901-a23c-99b22ade52dc"
            }
          ]
        },
        {
          "id": "a2ceac65-d253-40bd-9a60-eeb643962628",
          "name": "postUserBodyLogFat.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/body/log/fat.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create log entry for a body fat and get a response in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1c5893e-5f10-40fb-ad00-ea130ad58bcf"
            }
          ]
        },
        {
          "id": "f47d3f55-73cd-4185-8a23-18bd04791797",
          "name": "postUserBodyLogWeight.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/body/log/weight.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create log entry for a body weight using units in the unit system that corresponds to the Accept-Language header provided and get a response in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba0a31a2-c4c0-433f-9a0c-432f4f836b3f"
            }
          ]
        },
        {
          "id": "55518ad5-e23e-434d-b93e-a93717f38940",
          "name": "postUserBody.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/body.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Log body measurements using units in the unit system that corresponds to the Accept-Language header provided."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51dcee45-3428-402b-9f08-75a917ad9151"
            }
          ]
        },
        {
          "id": "8c8fcf8c-31b0-49fc-81ce-80b0f4cc8972",
          "name": "getUserUserBodyWeightDateStartDateOrEndDateEndDateOrPeriod.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/:user-id/body/weight/date/:start-date-or-end-date/:end-date-or-period.json"
              ],
              "variable": [
                {
                  "id": "user-id",
                  "value": "user-id",
                  "type": "string"
                },
                {
                  "id": "start-date-or-end-date",
                  "value": "start-date-or-end-date",
                  "type": "string"
                },
                {
                  "id": "end-date-or-period",
                  "value": "end-date-or-period",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get time series in the specified range for a given resource in the format requested using units in the unit system which corresponds to the Accept-Language header provided."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5dba89fb-d289-4f09-9f09-843ec0070862"
            }
          ]
        },
        {
          "id": "73752127-6941-4b43-bb73-00fa2601f189",
          "name": "getUserUserActivitiesCaloriesDateStartDateOrEndDateEndDateOrPeriod.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/:user-id/activities/calories/date/:start-date-or-end-date/:end-date-or-period.json"
              ],
              "variable": [
                {
                  "id": "user-id",
                  "value": "user-id",
                  "type": "string"
                },
                {
                  "id": "start-date-or-end-date",
                  "value": "start-date-or-end-date",
                  "type": "string"
                },
                {
                  "id": "end-date-or-period",
                  "value": "end-date-or-period",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get time series in the specified range for a given resource in the format requested using units in the unit system which corresponds to the Accept-Language header provided."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "470c9979-b19f-4292-b1bb-298c8726f2f2"
            }
          ]
        },
        {
          "id": "e6da40cd-c7b0-4a0b-b00d-44b9e1dbe11b",
          "name": "deleteUserBpBpLog.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/bp/:bp-log-id.json"
              ],
              "variable": [
                {
                  "id": "bp-log-id",
                  "value": "bp-log-id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete user's blood pressure log entry with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed5d4654-b276-405f-b412-4f346c890213"
            }
          ]
        },
        {
          "id": "33b429e2-462f-4bfc-9288-32d342f97d89",
          "name": "deleteUserHeartHeartLog.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/heart/:heart-log-id.json"
              ],
              "variable": [
                {
                  "id": "heart-log-id",
                  "value": "heart-log-id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete user's heart rate log entry with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a370134-ee5b-4953-9a80-b1a8a631038e"
            }
          ]
        },
        {
          "id": "8977c28b-1a90-4d6a-82f5-b5da1e35594e",
          "name": "deleteUserSleepSleepLog.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/sleep/:sleep-log-id.json"
              ],
              "variable": [
                {
                  "id": "sleep-log-id",
                  "value": "sleep-log-id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete user's sleep log entry with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53b3fc50-2784-463b-bd66-8af957e38888"
            }
          ]
        },
        {
          "id": "67b52bae-98dc-4ba6-bf2f-edf8071840ca",
          "name": "getUserUserBadges.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/:user-id/badges.json"
              ],
              "variable": [
                {
                  "id": "user-id",
                  "value": "user-id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get user's badges in the format requested. Response includes all badges for the user as seen on the Fitbit website badge locker (both activity and weight related). We return weight and distance badges based on the user's unit profile preference as on the website."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4357361-cf33-4899-93b3-6d6b6984b495"
            }
          ]
        },
        {
          "id": "6f01aff5-9eff-4b2b-bf3e-9a028e267f91",
          "name": "deleteUserActivitiesActivityLog.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/activities/:activity-log-id.json"
              ],
              "variable": [
                {
                  "id": "activity-log-id",
                  "value": "activity-log-id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete user's activity log entry with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7657329-f2ae-470d-a071-99dc7b22852a"
            }
          ]
        },
        {
          "id": "dc650a32-108a-4f98-b2ba-2b5fee9be2f7",
          "name": "deleteUserFoodsLogFoodLog.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/foods/log/:food-log-id.json"
              ],
              "variable": [
                {
                  "id": "food-log-id",
                  "value": "food-log-id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete the user's food log entry with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89c45bb8-d99d-4db2-9682-88cd4a6f3aaa"
            }
          ]
        },
        {
          "id": "db439afd-0352-4cee-a7e7-18abe8f04eef",
          "name": "postUserGlucose.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/glucose.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create log entry for a blood glucose measurement and/or HbA1c using units in the unit system which corresponds to the Accept-Language header provided and get a response in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1e7e69d-e6a4-412c-a9ae-3bf3f8d462ee"
            }
          ]
        },
        {
          "id": "32f9d60f-5507-40ff-ae0d-d66c3aec916e",
          "name": "postUserBp.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/bp.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create log entry for a blood pressure measurement and get a response in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75b5e251-5d50-492d-9d5d-881ee620a996"
            }
          ]
        },
        {
          "id": "1187c529-7700-4c04-b54e-db0ed932fe74",
          "name": "postUserHeart.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/heart.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create log entry for a heart rate measurement and get a response in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6733bfe8-9798-4fe9-9974-0dcc989848e2"
            }
          ]
        },
        {
          "id": "f0d391a9-22a8-4230-bdf4-6f5496e3b4ad",
          "name": "postUserSleep.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/sleep.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create log entry for a sleep and get a response in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10407399-0d69-4405-8dd8-b3b4ddf607b2"
            }
          ]
        },
        {
          "id": "0c58dd21-f66d-4883-97fb-1015c692ce75",
          "name": "postUserFoodsLog.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/foods/log.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create log entry for a food. You need to select one of the unit ids to create a food log entry. It is possible to fetch unit ids allowed for specific food via previous calls to endpoints that retrieve food lists of the user. Each unit id maps to a unit in the list returned via the Get Food Units API call."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a13372d-5004-41f3-bb62-51042215010a"
            }
          ]
        },
        {
          "id": "ba363777-c09c-4d7e-a11d-d7176e8a358c",
          "name": "getUserActivities.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/activities.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get user's activity statistics in the format requested using units in the unit system which corresponds to the Accept-Language header provided. Response contains both lifetime statistics from the tracker device and total numbers including the manual activity log entries as seen on the Fitbit website dashboard."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d19b439e-b431-43c3-a39b-c4c99d3f2a36"
            }
          ]
        },
        {
          "id": "93893abc-983b-455d-abd0-d4ab98186d9a",
          "name": "postUserActivities.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/activities.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create log entry for an activity using units in the unit system which corresponds to the Accept-Language header provided (or using optional custom distanceUnit)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d41b7a2-610a-46e6-a345-5b2879278011"
            }
          ]
        },
        {
          "id": "bf7cd0b2-f470-4037-a155-66b602e0497e",
          "name": "getUserFriendsLeaderboard.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/friends/leaderboard.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a leaderboard of user's friends progress in the format requested using units in the unit system which corresponds to the Accept-Language header provided. Authorized user himself is also included in the response."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7fc378d6-1177-45d6-9f0d-5fcdacac56c4"
            }
          ]
        },
        {
          "id": "2500a340-2fe1-4e26-8886-16b8c68f3447",
          "name": "getUserUserFriends.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/:user-id/friends.json"
              ],
              "variable": [
                {
                  "id": "user-id",
                  "value": "user-id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get user's friends in the format requested using units in the unit system which corresponds to the Accept-Language header provided."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b16705dc-4252-4266-9471-15a584d89c60"
            }
          ]
        },
        {
          "id": "01388a51-190f-487e-a8e7-39af0310595e",
          "name": "getUserGlucoseDateDate.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/glucose/date/:date.json"
              ],
              "variable": [
                {
                  "id": "date",
                  "value": "date",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of user's blood glucose and HbA1C measurements for a given day in the format requested using units in the unit system which corresponds to the Accept-Language header provided. Glucose measurement log entries are available only to authorized user. We always include all glucose trackers in the response body (with zero glucose value for the days with no measurements) to allow to seamlessly fetch a list of all additional user created custom trackers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97a22d93-e55d-45f9-8dfc-f126d86e053c"
            }
          ]
        }
      ]
    },
    {
      "name": "Foods",
      "item": [
        {
          "id": "c3a401d3-4fc6-4600-a8f3-a8303dd4943a",
          "name": "getFoodsUnits.json",
          "request": {
            "url": "http://api.fitbit.com/1/foods/units.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get list of all valid Fitbit food units in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1929aada-e239-4a02-b3a7-4a41b794da7d"
            }
          ]
        },
        {
          "id": "0c03b25c-4cd0-43b6-b602-ba8fa9562d21",
          "name": "getFoodsFood.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "foods/:food-id.json"
              ],
              "variable": [
                {
                  "id": "food-id",
                  "value": "food-id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the details of a specific food in Fitbit Food database (or private food for the user) in the format requested. Note, that nutritional values currently included in response only for the private foods."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bfc4f35b-7660-48e9-94c1-645b24f5a751"
            }
          ]
        }
      ]
    },
    {
      "name": "Activities",
      "item": [
        {
          "id": "fff9cd9c-7c9d-4b2a-ab29-619a791aa587",
          "name": "getActivities.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "activities/:id.json"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the details of a specific activity in Fitbit activities database in the format requested. If activity has levels, also get list of activity level details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c898bc70-afd1-40d3-92dc-b1e3ef8a7450"
            }
          ]
        }
      ]
    },
    {
      "name": "Activities.json",
      "item": [
        {
          "id": "b5f94fae-7ad3-40e9-8383-7c6ae4fb91e6",
          "name": "getActivities.json",
          "request": {
            "url": "http://api.fitbit.com/1/activities.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a tree of all valid Fitbit public activities from the activities catalog as well as private custom activities the user created in the format requested. If activity has levels, also get a list of activity level details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52e00e91-66d2-4575-8354-4f2e60b4759d"
            }
          ]
        }
      ]
    },
    {
      "name": "Foods.json",
      "item": [
        {
          "id": "00adb4b5-137b-488a-a9f5-73640a87e64e",
          "name": "postFoods.json",
          "request": {
            "url": "http://api.fitbit.com/1/foods.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create new private food for a user and get a response in a format requested. Created private food could be found in results of Search Foods call."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "731cf17a-662b-487a-a1b4-bdccd1deb7e7"
            }
          ]
        }
      ]
    }
  ]
}