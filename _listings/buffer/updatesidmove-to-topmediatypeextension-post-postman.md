{
  "info": {
    "name": "Buffer Post Updates Move To Top Mediatypeextension",
    "_postman_id": "ffdb7d82-cd8b-4bc3-bf14-7b161ca94af8",
    "description": "Move an existing status update to the top of the queue and recalculate times for all updates in the queue. Returns the update with its new posting time.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Info",
      "item": [
        {
          "id": "2dabecc4-7949-4f7f-914b-ac89c9cd42a4",
          "name": "returns-an-object-with-the-current-configuration-that-buffer-is-using-including-supported-services-t",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "info/configuration:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an object with the current configuration that Buffer is using, including supported services, their icons and the varying limits of character and schedules."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ee9638d-929e-40c8-be8a-946a103d1aba"
            }
          ]
        }
      ]
    },
    {
      "name": "Links",
      "item": [
        {
          "id": "795fac38-be41-4c07-929e-8e196012abfb",
          "name": "returns-an-object-with-a-the-numbers-of-shares-a-link-has-had-using-buffer-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "links/shares:mediaTypeExtension"
              ],
              "query": [
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an object with a the numbers of shares a link has had using Buffer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f73995af-f67e-4f66-b64c-320d4131efce"
            }
          ]
        }
      ]
    },
    {
      "name": "Profiles",
      "item": [
        {
          "id": "fc06e341-ec1a-4732-a703-0af866b2fc9e",
          "name": "set-the-posting-schedules-for-the-specified-social-media-profile-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "profiles/:id/schedules/update:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post Profiles Schedules Update Mediatypeextension"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e30fe7f7-96a1-415a-be19-3c40a062cd6b"
            }
          ]
        },
        {
          "id": "bb654a5c-abf8-4538-9cdc-ec14b1daf3b5",
          "name": "returns-details-of-the-posting-schedules-associated-with-a-social-media-profile-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "profiles/:id/schedules:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns details of the posting schedules associated with a social media profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "91424fa1-7c5d-41ff-a5c5-7b0a385e688b"
            }
          ]
        },
        {
          "id": "edd27696-2bca-408e-a1e5-f9dbcfaa2306",
          "name": "returns-an-array-of-updates-that-are-currently-in-the-buffer-for-an-individual-social-media-profile-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "profiles/:id/updates/pending:mediaTypeExtension"
              ],
              "query": [
                {
                  "key": "count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "since",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "utc",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Profiles Updates Pending Mediatypeextension"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "708854e4-248f-484a-bfb2-6df43cb76dfe"
            }
          ]
        },
        {
          "id": "8fb1500c-705e-48f4-988b-a0a7a3590bea",
          "name": "edit-the-order-at-which-statuses-for-the-specified-social-media-profile-will-be-sent-out-of-the-buff",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "profiles/:id/updates/reorder:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Edit the order at which statuses for the specified social media profile will be sent out of the buffer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dcdf6eef-b74e-4a0f-aee3-efb261670999"
            }
          ]
        },
        {
          "id": "f3fc7b08-e187-4d4a-8d5c-06545ead25b6",
          "name": "returns-an-array-of-updates-that-have-been-sent-from-the-buffer-for-an-individual-social-media-profi",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "profiles/:id/updates/sent:mediaTypeExtension"
              ],
              "query": [
                {
                  "key": "count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "since",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "utc",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an array of updates that have been sent from the buffer for an individual social media profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01b5b63d-acca-4f92-aa0b-82044ca72db3"
            }
          ]
        },
        {
          "id": "6f0a0812-5b47-419f-b3e7-812f811e66d9",
          "name": "randomize-the-order-at-which-statuses-for-the-specified-social-media-profile-will-be-sent-out-of-the",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "profiles/:id/updates/shuffle:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Randomize the order at which statuses for the specified social media profile will be sent out of the buffer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d6536b2-9715-4022-b47d-0baecf7f9dc1"
            }
          ]
        },
        {
          "id": "f09418f8-8ada-4e4f-be39-0f35c1810470",
          "name": "returns-details-of-the-single-specified-social-media-profile-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "profiles/:id:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns details of the single specified social media profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26e5eac3-bb89-41e8-98b4-220f3fce834b"
            }
          ]
        }
      ]
    },
    {
      "name": "ProfilesmediaTypeExtension",
      "item": [
        {
          "id": "2e5be23d-3da0-4444-b40c-a081bf21d20a",
          "name": "returns-an-array-of-social-media-profiles-connected-to-a-users-account-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "profiles:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an array of social media profiles connected to a users account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2aa5bc67-5d2e-477c-9daf-38f7fc7eac71"
            }
          ]
        }
      ]
    },
    {
      "name": "Updates",
      "item": [
        {
          "id": "66bb8df6-5950-45a2-8c12-61b881a7bc31",
          "name": "create-one-or-more-new-status-updates-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "updates/create:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create one or more new status updates."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd7c9bc3-7092-4d9c-9124-7c74cdd62a47"
            }
          ]
        },
        {
          "id": "2947959d-5e28-4e43-9fa5-8787584fcd30",
          "name": "permanently-delete-an-existing-status-update-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "updates/:id/destroy:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Permanently delete an existing status update."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dfad0d0a-869e-4070-9679-2e2ba16b3e84"
            }
          ]
        },
        {
          "id": "74cc05cd-2f60-46fa-9dee-01910e39cb5e",
          "name": "returns-the-detailed-information-on-individual-interactions-with-the-social-media-update-such-as-fav",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "updates/:id/interactions:mediaTypeExtension"
              ],
              "query": [
                {
                  "key": "count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "event",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the detailed information on individual interactions with the social media update such as favorites, retweets and likes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1040da9c-1373-4c87-9b0d-e9964c753d82"
            }
          ]
        },
        {
          "id": "709a184d-12ee-4106-bc5e-4fea4ac03e46",
          "name": "move-an-existing-status-update-to-the-top-of-the-queue-and-recalculate-times-for-all-updates-in-the-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "updates/:id/move_to_top:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Move an existing status update to the top of the queue and recalculate times for all updates in the queue. Returns the update with its new posting time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f22c540a-608c-40f5-ba2e-432c2cd0ad78"
            }
          ]
        }
      ]
    }
  ]
}