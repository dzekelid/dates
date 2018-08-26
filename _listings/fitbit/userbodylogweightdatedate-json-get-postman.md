{
  "info": {
    "name": "Fitbit Get User Body Log Weight Date Date .json",
    "_postman_id": "a97367c3-b569-4ab2-a145-010ac055a0f6",
    "description": "Get a list of all user's body weight log entries for a given day in the format requested using units in the unit system which corresponds to the Accept-Language header provided.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "4fd5afe4-21a5-4098-9893-0a1928815ff9",
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
              "id": "954e28b0-73fe-47ed-af07-a307e3cd3ed3"
            }
          ]
        },
        {
          "id": "8b07b1b8-bd83-430f-b90f-8349f97f7050",
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
              "id": "8048cc7d-aac5-40ed-851d-55e5efae1e5a"
            }
          ]
        },
        {
          "id": "9dfef69c-4839-4a16-b2b6-e9b3533a0c26",
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
              "id": "623aadc4-9fcc-430e-8e6d-300e74767a39"
            }
          ]
        },
        {
          "id": "40ec6669-11ed-4a5e-b834-7e4960fcf855",
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
              "id": "3fe7fd87-f3fb-4d24-891a-5c26d02ded71"
            }
          ]
        },
        {
          "id": "e8ba7f3e-0c90-4cac-adf7-121d324bbdc5",
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
              "id": "515582b8-6be6-4176-b27a-ae0d3ed6b916"
            }
          ]
        },
        {
          "id": "9214fc61-3be8-4c50-8d49-94280fd138d7",
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
              "id": "6a5bf1f6-8fc9-4499-9565-fd114c130238"
            }
          ]
        },
        {
          "id": "6baeaa27-6cd9-41a0-9814-ed103e70c054",
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
              "id": "18fb7705-644b-4f47-99ef-db31884df490"
            }
          ]
        },
        {
          "id": "7f45ad7b-146b-47f3-96fd-62519e7cb402",
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
              "id": "aaad39a0-a7ff-4309-84f4-2a212254fbf2"
            }
          ]
        },
        {
          "id": "6b4ca664-2910-4e7b-ada3-25eb463c7760",
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
              "id": "03732a3f-78c9-48f3-9ba0-e7eed152bd6f"
            }
          ]
        },
        {
          "id": "d919a81d-0dd6-4cec-a0af-ffe09503e772",
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
              "id": "0d109c42-cab3-4502-b88e-9efbd5b1a8c2"
            }
          ]
        },
        {
          "id": "9920381c-6f07-41ab-a7f7-d33b833692fa",
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
              "id": "49f45d31-3613-4031-ab15-6145190ba932"
            }
          ]
        },
        {
          "id": "f59cd67a-d213-43de-8e51-5cc6fa881f40",
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
              "id": "2629480a-d3fa-41ac-93c1-39c861c6b141"
            }
          ]
        },
        {
          "id": "882cc2f3-a637-4410-8546-a945e5f8f725",
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
              "id": "2ba66c32-6f8b-4743-af1e-d0a1d2124eec"
            }
          ]
        },
        {
          "id": "540630c0-43a3-4a4f-96d5-486d35aabbbe",
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
              "id": "a3b3eaed-1162-42d5-9f5d-632057e69a14"
            }
          ]
        },
        {
          "id": "96f4a840-4330-4e32-969a-c607ffb496c6",
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
              "id": "54c68eca-520d-4665-9927-a00f13a54bb1"
            }
          ]
        },
        {
          "id": "0fcd9d9e-b22b-4640-90e1-8b700616af76",
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
              "id": "bf858233-1428-41a2-b558-39de1e8f8cf9"
            }
          ]
        },
        {
          "id": "a25884b7-b69a-4401-8ac7-40ab495d3da8",
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
              "id": "9d412ab1-90c9-4fe3-9a1d-5355e0ca31ff"
            }
          ]
        },
        {
          "id": "e8ee0be6-1f7b-4a1f-85de-14ae713fb772",
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
              "id": "21c880b7-f4b4-4f7b-a9e4-7d49950439c6"
            }
          ]
        },
        {
          "id": "b4c396fd-f343-4b14-a1d3-3b1429481a67",
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
              "id": "7e63c495-c03c-4ca0-91d2-34dc0445792e"
            }
          ]
        },
        {
          "id": "c56a0d10-5796-4346-b72e-2d06152d6bea",
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
              "id": "a0f69b3f-f405-4760-9719-e82ef244cc92"
            }
          ]
        },
        {
          "id": "baaa32bf-e248-4f4e-b50c-bab3dfb7b099",
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
              "id": "3a4a7066-8934-4992-878a-7c8edfca1bea"
            }
          ]
        },
        {
          "id": "2666a6ac-6d93-4a89-aea3-e69c7f56b903",
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
              "id": "c80b9b9a-ddc4-4761-901d-d58f628f09a6"
            }
          ]
        },
        {
          "id": "b45e19bd-404f-47b2-81e2-dba662689f7f",
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
              "id": "3b4d7553-dacd-4925-8c44-086dfb10cb48"
            }
          ]
        },
        {
          "id": "a5b53a42-eb2f-4d3e-abd2-878224c3c497",
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
              "id": "6a1dbb51-2b67-476a-ba5c-0bb75ab0db73"
            }
          ]
        },
        {
          "id": "ab5eca6b-32d2-419a-bee1-0594e09a34e8",
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
              "id": "ff6a7ef7-1821-4e1a-b075-bdc5dd88c249"
            }
          ]
        },
        {
          "id": "733e9866-5639-4fcd-8119-8c9ab793102d",
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
              "id": "7f10d760-9b96-43c2-9329-40555e561f0f"
            }
          ]
        },
        {
          "id": "4fa188a6-2052-4a70-8066-4278ca6e586b",
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
              "id": "07946889-de90-43f0-a93c-cad73f851422"
            }
          ]
        },
        {
          "id": "b357aab6-ae18-4ce5-a7b5-da6e2c39168d",
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
              "id": "ed165136-fc75-4c43-8236-52e6187fe214"
            }
          ]
        },
        {
          "id": "83eaa437-e3db-4cc0-94a0-a030d4b720d9",
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
              "id": "214f19db-0501-4e2a-95c8-bf34070c6584"
            }
          ]
        },
        {
          "id": "ec355af3-42c3-41f7-803c-46f057ee1b0d",
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
              "id": "59b0d069-b62f-41a1-859a-2b75df8b57a8"
            }
          ]
        },
        {
          "id": "967e9b47-43ec-4b6b-b532-e16f25373767",
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
              "id": "535d49b6-1cd6-40f3-9da3-46d31d366244"
            }
          ]
        },
        {
          "id": "8d3c40ed-9cdd-4142-8ff7-a0b61df09002",
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
              "id": "2f4351bb-0ff3-49b4-9356-3c761c7ac408"
            }
          ]
        },
        {
          "id": "9d3c0f5a-2e93-4d8d-9e97-98c5a10e0626",
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
              "id": "ab2553f1-527e-41ee-a1f7-ff701a130a0a"
            }
          ]
        },
        {
          "id": "aaa76316-99be-4f5f-b5e8-e93afde46462",
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
              "id": "b5210d8f-08b7-4c38-9107-0865eee59d3e"
            }
          ]
        },
        {
          "id": "0320556c-001d-4b3d-981b-320c21be39d9",
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
              "id": "e394b0ed-3345-4038-a3c3-8e1abd97a83d"
            }
          ]
        },
        {
          "id": "c751ab71-1da7-4093-ab0b-8345c3a8e7a7",
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
              "id": "68a681d5-12b8-4c76-8a63-5e1413d203d9"
            }
          ]
        },
        {
          "id": "2330f784-f0a2-43b7-af98-28849a6df3cd",
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
              "id": "2ef07759-6b4c-41ca-9bdc-1488b46763ac"
            }
          ]
        },
        {
          "id": "ae2dc419-9279-4d79-800e-8cd682ade78e",
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
              "id": "0cf1a44d-462d-48b8-aabb-654edee69aa9"
            }
          ]
        },
        {
          "id": "450f4030-e6b0-488a-a939-fb5c6adc53b3",
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
              "id": "7bd39d70-a57b-4ceb-88fa-7ad6841ac1d4"
            }
          ]
        },
        {
          "id": "440868de-dfb9-4f11-a0be-96d13422ca52",
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
              "id": "5863efe4-6ccc-4ba7-b75f-4eb9f0f09116"
            }
          ]
        },
        {
          "id": "effaf017-115f-4787-b8b2-539207ae5303",
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
              "id": "e98ae56f-0d09-4c4a-8961-b3342b392c24"
            }
          ]
        },
        {
          "id": "bbca8bf4-a130-4dce-bbc8-dae287d2b866",
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
              "id": "7c68efb7-d061-436e-b44c-1431a5bd3196"
            }
          ]
        },
        {
          "id": "d34c0f3a-c0d8-445d-ac9f-fc87b50e36c4",
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
              "id": "2d2ed852-fa25-41c9-93f8-db9f364b1183"
            }
          ]
        },
        {
          "id": "f1ba95af-5342-411d-bf9a-31ad90b707a1",
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
              "id": "67e869e6-92f5-44f9-a15d-e7280c4029bc"
            }
          ]
        },
        {
          "id": "6b3bafde-84c4-40e1-8a43-9c464b283dfa",
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
              "id": "2d774ae7-4a63-4b8e-a8c4-8512fb0364ac"
            }
          ]
        },
        {
          "id": "342f6177-0e28-4900-a4b9-b009f91005fa",
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
              "id": "16fa9fcc-b2b7-4b4f-b7d2-43d4dd3e8f17"
            }
          ]
        },
        {
          "id": "70657d68-5d5e-45af-b83a-e55d0e3324a9",
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
              "id": "a5a844d2-c563-4eab-988a-1d58dcdeb660"
            }
          ]
        },
        {
          "id": "bd74637c-775a-4974-8aba-41420fa52a1f",
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
              "id": "bf9e6cec-53ab-4839-b14a-0f2aa48b37a5"
            }
          ]
        },
        {
          "id": "46314746-3d43-4d87-8ae3-f09fa606a5c0",
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
              "id": "06d389bc-6d77-4266-8568-1484b753f90c"
            }
          ]
        },
        {
          "id": "0a742c17-bdc2-4bd5-af25-8011888f8899",
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
              "id": "7652d0b3-fe8e-45b5-975f-7091027a78e8"
            }
          ]
        },
        {
          "id": "893d344f-0be7-411e-b473-3be65ad8c2e0",
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
              "id": "7277d4c5-0627-4eb3-bbbe-7903d7e6fee2"
            }
          ]
        },
        {
          "id": "f3f0c867-4a3f-45c0-8908-0b5d1a86b000",
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
              "id": "0b5e14c8-b679-4ce9-8c60-07bf2a30f648"
            }
          ]
        },
        {
          "id": "6941c077-e5bc-4eee-8a45-67f71cdd605b",
          "name": "getUserBpDateDate.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/bp/date/:date.json"
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
            "description": "Get an average value and a list of user's blood pressure log entries for a given day in the format requested. Blood pressure log entries are available only to authorized user. Blood pressure log entries in response are sorted exactly the same as they are presented on the Fitbit website."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0f9eb0c-ec62-43ea-b6f6-f43986185e19"
            }
          ]
        },
        {
          "id": "ca4d184d-70f7-48f2-93c8-f585ab6d58d5",
          "name": "getUserHeartDateDate.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/heart/date/:date.json"
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
            "description": "Get an average values and a list of user's heart rate log entries for a given day in the format requested. Heart rate data available only to the authorized user. Heart rate log entries in response are sorted exactly the same as they are presented on the Fitbit website. We always include all heart rate trackers in the \"average\" section of the response body (with zero average values for the days with no measurements) to allow to seamlessly fetch a list of all additional user created custom trackers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6937c08-494c-41c8-b737-79b1050f3972"
            }
          ]
        },
        {
          "id": "d1538eaa-2820-4c6d-a061-807b9928f2bc",
          "name": "getUserUserSleepDateDate.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/:user-id/sleep/date/:date.json"
              ],
              "variable": [
                {
                  "id": "user-id",
                  "value": "user-id",
                  "type": "string"
                },
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
            "description": "Get a summary and list of a user's sleep log entries for a given day in the format requested. Endpoint returns summary for all sleep log entries for the given day (including naps). If you need data only for the main sleep you can fetch entry with \"isMainSleep\" = true or use Get-Time-Series calls."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "340191bd-6de4-49f5-a047-258d61fe455f"
            }
          ]
        },
        {
          "id": "3d0648e9-2c7e-4dd4-9380-adf2181fd100",
          "name": "getUserUserFoodsLogDateDate.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/:user-id/foods/log/date/:date.json"
              ],
              "variable": [
                {
                  "id": "user-id",
                  "value": "user-id",
                  "type": "string"
                },
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
            "description": "Get a summary and list of a user's food log entries for a given day in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e725852d-f84f-4528-93a4-5d9a9c874367"
            }
          ]
        },
        {
          "id": "299fb6e8-3dc7-4c6c-a949-e85b93c20d89",
          "name": "getUserUserActivitiesDateDate.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/:user-id/activities/date/:date.json"
              ],
              "variable": [
                {
                  "id": "user-id",
                  "value": "user-id",
                  "type": "string"
                },
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
            "description": "Get a summary and list of a user's activities and activity log entries for a given day in the format requested using units in the unit system which corresponds to the Accept-Language header provided."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b080698-ac73-44d7-88ee-df939f3342be"
            }
          ]
        },
        {
          "id": "4d9548b9-8a70-40f9-8c74-059e74c0c3b5",
          "name": "getUserBodyLogFatDateDate.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/body/log/fat/date/:date.json"
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
            "description": "Get a list of all user's body fat log entries for a given day in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48ae6016-2aca-43d1-93a0-34674bf1f37b"
            }
          ]
        },
        {
          "id": "398dbeca-ba50-47b8-af4b-a3717ea41432",
          "name": "getUserBodyLogWeightDateDate.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "user/-/body/log/weight/date/:date.json"
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
            "description": "Get a list of all user's body weight log entries for a given day in the format requested using units in the unit system which corresponds to the Accept-Language header provided."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e763419-dc5d-4977-8950-7bc2397cd767"
            }
          ]
        }
      ]
    },
    {
      "name": "Foods",
      "item": [
        {
          "id": "fbfa970f-1975-4c9e-a23b-331e403aa272",
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
              "id": "ef9d6bc4-8ac3-41e6-b8ff-8560aadde011"
            }
          ]
        },
        {
          "id": "99e3ac35-9a46-4fde-b710-be7e2ee7d4d7",
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
              "id": "a8682645-2be6-4a0a-a3ba-659125594967"
            }
          ]
        }
      ]
    },
    {
      "name": "Activities",
      "item": [
        {
          "id": "545fbc45-94c5-4d63-b22b-74d3076b2a4e",
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
              "id": "98430b08-be7c-411f-8ae7-de683533f534"
            }
          ]
        }
      ]
    },
    {
      "name": "Activities.json",
      "item": [
        {
          "id": "65487668-ec63-4f72-b06f-36dd324e9383",
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
              "id": "bde270b0-668f-490f-9618-fea947a72b14"
            }
          ]
        }
      ]
    },
    {
      "name": "Foods.json",
      "item": [
        {
          "id": "6e5e6f81-e162-4fcd-bb02-3ff79f192582",
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
              "id": "836c9ca2-0b3c-4b35-9658-4419ea04e763"
            }
          ]
        }
      ]
    }
  ]
}