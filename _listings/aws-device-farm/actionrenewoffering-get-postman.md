{
  "info": {
    "name": "AWS Device Farm API Renew Offering",
    "_postman_id": "3d6498aa-ee08-475c-b4c3-742656554ea9",
    "description": "Explicitly sets the quantity of devices to renew for an offering, starting from the\n      effectiveDate of the next period.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device Pool",
      "item": [
        {
          "id": "8180aafe-2f93-4649-814b-d42894555285",
          "name": "createDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=CreateDevicePool?description=description&name=name&projectArn=projectArn&rules=rules",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2337976-1628-48db-8ade-72b2b978954b"
            }
          ]
        },
        {
          "id": "5c6653aa-931f-46a5-a8be-7a006fcf459b",
          "name": "deleteDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDevicePool?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a device pool given the pool ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd40bb44-95c7-4eac-be72-550bff6ed1d6"
            }
          ]
        },
        {
          "id": "959ce113-921e-4c9d-bd51-1731eb34a229",
          "name": "getDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=GetDevicePool?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6cdfcda-20ac-493f-8494-b57d3d5b5f14"
            }
          ]
        },
        {
          "id": "8e339e80-4ec1-478f-b91b-79bd01b154c5",
          "name": "getDevicePoolCompatibility",
          "request": {
            "url": "http://example.com/api/?Action=GetDevicePoolCompatibility?appArn=appArn&devicePoolArn=devicePoolArn&testType=testType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about compatibility with a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88702ecd-1794-4888-bc30-cd60c333c895"
            }
          ]
        },
        {
          "id": "591cf103-1d04-41af-ba33-3fb58948d1ed",
          "name": "listDevicePools",
          "request": {
            "url": "http://example.com/api/?Action=ListDevicePools?arn=arn&nextToken=nextToken&type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about device pools."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "368a5f12-afa6-487f-8b90-ad0d219ffd6e"
            }
          ]
        }
      ]
    },
    {
      "name": "Project",
      "item": [
        {
          "id": "f3c0f6f3-7b88-4369-bfc7-979de6b1d708",
          "name": "createProject",
          "request": {
            "url": "http://example.com/api/?Action=CreateProject?name=name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e81ad95-e843-4910-9de6-39cdac609a61"
            }
          ]
        }
      ]
    },
    {
      "name": "Remote Access Sessions",
      "item": [
        {
          "id": "27949f80-c67f-4197-bcb2-4f862b7d1eb9",
          "name": "createRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=CreateRemoteAccessSession?configuration=configuration&deviceArn=deviceArn&name=name&projectArn=projectArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Specifies and starts a remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6030353-6405-46a7-b8df-7667ccd78714"
            }
          ]
        },
        {
          "id": "9e004dbe-9895-4cca-99d1-59ad04f5c25e",
          "name": "deleteRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRemoteAccessSession?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a completed remote access session and its results."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8a072e2-e3c0-4913-b6ad-c24eb977ae13"
            }
          ]
        },
        {
          "id": "4e5bc1e2-791b-44ba-9dd4-d4beb0211c53",
          "name": "getRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=GetRemoteAccessSession?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a link to a currently running remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c4e6c93-96d6-49eb-ab5c-0d693eb4c593"
            }
          ]
        },
        {
          "id": "ad878fd6-adae-4be6-bc39-cd25b63ac200",
          "name": "installToRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=InstallToRemoteAccessSession?appArn=appArn&remoteAccessSessionArn=remoteAccessSessionArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Installs an application to the device in a remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f53f3878-3e3c-4a1c-8c3a-8fc660fb8af4"
            }
          ]
        },
        {
          "id": "98e6541f-5add-42ba-98d0-0ba89b4b1849",
          "name": "listRemoteAccessSessions",
          "request": {
            "url": "http://example.com/api/?Action=ListRemoteAccessSessions?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all currently running remote access sessions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "599c351d-7428-4936-bacd-36511e6738b1"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "7401ac18-8152-4b36-b8df-e93f34882f27",
          "name": "createUpload",
          "request": {
            "url": "http://example.com/api/?Action=CreateUpload?contentType=contentType&name=name&projectArn=projectArn&type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Uploads an app or test scripts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10199678-0f7d-41de-97e9-f5f58ae06c0f"
            }
          ]
        },
        {
          "id": "b661abc4-59dc-4d8b-be17-0f2199208ea8",
          "name": "getUpload",
          "request": {
            "url": "http://example.com/api/?Action=GetUpload?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about an upload."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5442944-91fb-4aea-b5f4-8fb316f26574"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "ed60ee01-327a-4105-a525-5982210e9310",
          "name": "deleteProject",
          "request": {
            "url": "http://example.com/api/?Action=DeleteProject?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an AWS Device Farm project, given the project ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92a3015e-5300-4c87-9469-2f326c824553"
            }
          ]
        },
        {
          "id": "388b7381-eef2-4ee4-8c45-5d2e698b96d0",
          "name": "getProject",
          "request": {
            "url": "http://example.com/api/?Action=GetProject?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95aba6bc-b626-489a-a8a2-2572aa4e3077"
            }
          ]
        },
        {
          "id": "8c3743cb-385d-49e4-939c-c4e9317359b5",
          "name": "listProjects",
          "request": {
            "url": "http://example.com/api/?Action=ListProjects?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about projects."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e05db665-b640-49e9-86cb-d261983cc4b6"
            }
          ]
        }
      ]
    },
    {
      "name": "Runs",
      "item": [
        {
          "id": "76acc781-aef9-4744-8fed-a05d962e0c48",
          "name": "deleteRun",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRun?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the run, given the run ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2fd125e4-9514-45af-837b-608abc2698e2"
            }
          ]
        },
        {
          "id": "5ceb262e-fa29-43e8-8bd2-a213e0b3a934",
          "name": "getRun",
          "request": {
            "url": "http://example.com/api/?Action=GetRun?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e15e34d-ce6e-4764-80a0-e7b64ac02e45"
            }
          ]
        },
        {
          "id": "762c511e-9137-4a15-9978-3c5ab534c830",
          "name": "listRuns",
          "request": {
            "url": "http://example.com/api/?Action=ListRuns?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about runs, given an AWS Device Farm project ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c00f3170-8cb6-4d27-88e4-b1c1dc318a56"
            }
          ]
        }
      ]
    },
    {
      "name": "Uploads",
      "item": [
        {
          "id": "462e53fe-8668-4523-8d8c-28f3808b5f8e",
          "name": "deleteUpload",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUpload?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an upload given the upload ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ecd8f31e-4903-436a-88bf-3ebfa31594b4"
            }
          ]
        },
        {
          "id": "427e2bc3-47cb-4eb6-9c52-aa1f457bc111",
          "name": "listUploads",
          "request": {
            "url": "http://example.com/api/?Action=ListUploads?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about uploads, given an AWS Device Farm project ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b4c58cf-21ac-4d5a-bed8-6aedbda07a8e"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Settings",
      "item": [
        {
          "id": "2434006e-195e-4eda-b53f-a98e868d97e2",
          "name": "getAccountSettings",
          "request": {
            "url": "http://example.com/api/?Action=GetAccountSettings?accountSettings=accountSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the number of unmetered iOS and/or unmetered Android devices that have been purchased by the account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8cad699-5d00-46bb-8c73-96475ffb3954"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "520322ce-0f55-492d-aefc-8d4b4182f157",
          "name": "getDevice",
          "request": {
            "url": "http://example.com/api/?Action=GetDevice?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a unique device type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "053a82a2-7c9e-47a6-8dae-0272d8c1ab0b"
            }
          ]
        },
        {
          "id": "fa4be916-d21c-4c7b-ac8e-83c9895f85ce",
          "name": "listDevices",
          "request": {
            "url": "http://example.com/api/?Action=ListDevices?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about unique device types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aafd3097-0cfc-404e-b3ce-dd42b639aeed"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "c7c41fd5-b925-41a7-9551-c9dfe0d4ed4f",
          "name": "getJob",
          "request": {
            "url": "http://example.com/api/?Action=GetJob?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfe7d7cd-dcb2-4e48-957e-414f45661deb"
            }
          ]
        },
        {
          "id": "d48dd84d-b2be-4abb-b03e-f4f1292132e3",
          "name": "listJobs",
          "request": {
            "url": "http://example.com/api/?Action=ListJobs?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about jobs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a032221e-e3dc-4f5a-9a86-ea04d6ca41ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Offering Status",
      "item": [
        {
          "id": "b5f163c3-f015-4720-9d6c-8866ecb4a576",
          "name": "getOfferingStatus",
          "request": {
            "url": "http://example.com/api/?Action=GetOfferingStatus?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the current status and future status of all offerings purchased by an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5c7c215-9bb3-45f0-a2af-9beb50fb8add"
            }
          ]
        }
      ]
    },
    {
      "name": "Suites",
      "item": [
        {
          "id": "c9a2291f-3ff3-4119-8e0a-da84ef5b0d9b",
          "name": "getSuite",
          "request": {
            "url": "http://example.com/api/?Action=GetSuite?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a suite."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6897fa9b-524a-43fb-87aa-d05d54dc052a"
            }
          ]
        },
        {
          "id": "d112b9ce-eb91-4ce9-9784-857621a07eae",
          "name": "listSuites",
          "request": {
            "url": "http://example.com/api/?Action=ListSuites?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about suites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a76a66b4-498c-48eb-902d-cd6017c816dd"
            }
          ]
        }
      ]
    },
    {
      "name": "Tests",
      "item": [
        {
          "id": "18846989-fbd1-4d44-b404-416eee2ab891",
          "name": "getTest",
          "request": {
            "url": "http://example.com/api/?Action=GetTest?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a test."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "542e5b3d-0674-4a6c-ae2c-7edee54b3f8a"
            }
          ]
        },
        {
          "id": "b28c1ab7-0356-423b-9399-8c660662c953",
          "name": "listTests",
          "request": {
            "url": "http://example.com/api/?Action=ListTests?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about tests."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf4594f7-9283-4880-96a3-9747c6808f5e"
            }
          ]
        }
      ]
    },
    {
      "name": "Artifacts",
      "item": [
        {
          "id": "8650f14f-aa2c-496c-bef8-b8902bfe7788",
          "name": "listArtifacts",
          "request": {
            "url": "http://example.com/api/?Action=ListArtifacts?arn=arn&nextToken=nextToken&type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about artifacts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1287f11f-1510-43f8-af1a-3954b89bb3dc"
            }
          ]
        }
      ]
    },
    {
      "name": "Offerings",
      "item": [
        {
          "id": "84d7eb9b-d2db-4f4a-964d-a3aa9c941941",
          "name": "listOfferings",
          "request": {
            "url": "http://example.com/api/?Action=ListOfferings?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of products or offerings that the user can manage through the API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4598a1e9-e0f9-44aa-a68c-aa4ec4235336"
            }
          ]
        },
        {
          "id": "66208df7-fb4a-4c23-828e-3ac478268e05",
          "name": "purchaseOffering",
          "request": {
            "url": "http://example.com/api/?Action=PurchaseOffering?offeringId=offeringId&quantity=quantity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Immediately purchases offerings for an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b900fb1-6ad2-42a2-be7c-fbf48f0a1618"
            }
          ]
        },
        {
          "id": "cb5dce4e-1633-4cf5-9939-db07249e08b6",
          "name": "renewOffering",
          "request": {
            "url": "http://example.com/api/?Action=RenewOffering?offeringId=offeringId&quantity=quantity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Explicitly sets the quantity of devices to renew for an offering, starting from the\n      effectiveDate of the next period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cdded76-dbc1-4b2d-9c46-9902654ecba9"
            }
          ]
        }
      ]
    },
    {
      "name": "Offering Transactions",
      "item": [
        {
          "id": "a70442f4-4fc3-4f3c-85a0-c7b024bca1a6",
          "name": "listOfferingTransactions",
          "request": {
            "url": "http://example.com/api/?Action=ListOfferingTransactions?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all historical purchases, renewals, and system renewal transactions for an\n      AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62417938-1d3f-4a55-bd85-621edde5ab56"
            }
          ]
        }
      ]
    },
    {
      "name": "Samples",
      "item": [
        {
          "id": "7260fb92-6864-438f-8441-e322cf4e5a00",
          "name": "listSamples",
          "request": {
            "url": "http://example.com/api/?Action=ListSamples?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about samples, given an AWS Device Farm project ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1987f25-0507-4394-acf1-edfdf257cc0d"
            }
          ]
        }
      ]
    },
    {
      "name": "Unique Problems",
      "item": [
        {
          "id": "dcc4bb49-553c-49f4-8ac5-e58cf0e36f26",
          "name": "listUniqueProblems",
          "request": {
            "url": "http://example.com/api/?Action=ListUniqueProblems?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about unique problems."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1429013-624d-4729-9fbb-2ac49bbd1e84"
            }
          ]
        }
      ]
    }
  ]
}