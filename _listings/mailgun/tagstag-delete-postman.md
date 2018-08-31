{
  "info": {
    "name": "Mailgun API Delete Tag",
    "_postman_id": "071537ad-c858-48bb-874e-d9343a63ad0d",
    "description": "Deletes all counters for particular tag and the tag itself.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bounces",
      "item": [
        {
          "id": "6b3096c6-3094-4b26-8228-570a1b8b6def",
          "name": "getBounces",
          "request": {
            "url": "http://api.mailgun.net/v2/bounces/?limit=%7B%7D&skip=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches the list of bounces."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f618f6b5-c7d4-42ac-8f31-292335a902e2"
            }
          ]
        }
      ]
    },
    {
      "name": "Bounce",
      "item": [
        {
          "id": "7f911b36-9880-4957-b6cd-e963380cf217",
          "name": "postBounces",
          "request": {
            "url": "http://api.mailgun.net/v2/bounces/?address=%7B%7D&code=%7B%7D&error=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a permanent bounce to the bounces table. Updates the existing record if already here."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ef8a364-149f-4017-b5e7-ccaf0cea9817"
            }
          ]
        },
        {
          "id": "48ee207a-3c65-4512-b176-9f8212fd9e43",
          "name": "getBouncesAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "bounces/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a single bounce event by a given email address. This is useful to check if a given email address has bounced before."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1df1a9a4-5a35-4c21-8d78-7881fecdda03"
            }
          ]
        },
        {
          "id": "a07f9f1c-9c10-4fa6-856e-0ca9a3fb3df3",
          "name": "deleteBouncesAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "bounces/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "address",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Clears a bounce event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89206af1-8212-4a91-8d80-437efba76bef"
            }
          ]
        }
      ]
    },
    {
      "name": "Complaints",
      "item": [
        {
          "id": "bfcba39f-3df8-4e8b-b3eb-92d71c6e35f3",
          "name": "getComplaints",
          "request": {
            "url": "http://api.mailgun.net/v2/complaints/?limit=%7B%7D&skip=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches the list of complaints."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00ab2f7e-4ff2-4e5d-b5bc-6226a60e2b7a"
            }
          ]
        }
      ]
    },
    {
      "name": "Complaint",
      "item": [
        {
          "id": "693c4579-9c22-4661-8374-214dff10e730",
          "name": "postComplaints",
          "request": {
            "url": "http://api.mailgun.net/v2/complaints/?address=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds an address to the complaints table."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5decf6e8-14dc-4a2a-a3ba-2c866145cda3"
            }
          ]
        },
        {
          "id": "1a08e67f-41ce-408f-8ce0-15be9da15d1e",
          "name": "getComplaintsAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "complaints/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a single spam complaint by a given email address. This is useful to check if a particular user has complained."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebffe9c6-df83-4b99-a832-9a0484afc82e"
            }
          ]
        },
        {
          "id": "01cec12a-50ad-4a6b-aae0-aab119ecbd53",
          "name": "deleteComplaintsAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "complaints/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a given spam complaint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39ac56c3-8624-4271-be78-f1cddc61edf7"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "b04c1c4c-637b-4093-b6a2-d8d67064bac0",
          "name": "postLists",
          "request": {
            "url": "http://api.mailgun.net/v2/lists?access_level=%7B%7D&address=%7B%7D&description=%7B%7D&name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new mailing list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dbbeb400-debe-4c5e-bdff-3d1c98bbf32f"
            }
          ]
        },
        {
          "id": "eb6ca674-3f31-457d-94f8-05fb919cc94f",
          "name": "getListsAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "lists/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a single mailing list by a given address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f08fff85-7847-4dda-8ff8-9e30d882b7e5"
            }
          ]
        },
        {
          "id": "2d3c2abc-5bb5-457a-a974-4f32364774a8",
          "name": "putListsAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "lists/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "address",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update mailing list properties, such as address, description or name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "147e6700-a789-4268-b4f5-78f3f9950cc4"
            }
          ]
        },
        {
          "id": "b7bc3608-995d-4a79-8685-f3e3863585ed",
          "name": "deleteListsAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "lists/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a mailing list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5f8c68a-4703-4d6f-b395-baa3fbda6b73"
            }
          ]
        },
        {
          "id": "3fadf3c8-3326-4f7e-9bbf-4fee38d0e1f2",
          "name": "getListsAddressMembers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "lists/:address/members"
              ],
              "query": [
                {
                  "key": "Name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "subscribed",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "upsert",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "vars",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a member to the mailing list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e93e6423-959a-4b90-a442-e5e40ab264f9"
            }
          ]
        },
        {
          "id": "b99aa776-70ab-4caf-9f2d-e834f7478807",
          "name": "getListsAddressMembers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "lists/:address/members/"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "skip",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "subscribed",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "address",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches the list of mailing list members."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b196604-95a0-4a6b-9093-3fb5c983d759"
            }
          ]
        },
        {
          "id": "115b4a74-44d7-4fb7-99ff-7bd59503c3f4",
          "name": "getListsAddressMembersMemberAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "lists/:address/members/:member_address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "member_address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a mailing list member."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57671ee3-9893-4796-8fb3-89fb4cd03fe5"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "9201e337-9067-47bc-b883-a5ead0ca8eff",
          "name": "getLists",
          "request": {
            "url": "http://api.mailgun.net/v2/lists/?access_level=%7B%7D&address=%7B%7D&description=%7B%7D&limit=%7B%7D&namespace_id=%7B%7D&skip=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of mailing lists under your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10bdaefb-8e35-49cd-9315-179ab354b08a"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "ca3dc7c4-cf21-4dbb-9b1e-3554bddfe4fc",
          "name": "postMessages.mime",
          "request": {
            "url": "http://api.mailgun.net/v2/messages.mime?h:X-My-Header=%7B%7D&message=%7B%7D&o:campaign=%7B%7D&o:deliverytime=%7B%7D&o:dkim=%7B%7D&o:tag=%7B%7D&o:testmode=%7B%7D&o:tracking=%7B%7D&o:tracking-clicks=%7B%7D&o:tracking-opens=%7B%7D&to=%7B%7D&v:my-var=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a message in MIME format. Note: you will need to build a MIME string yourself. Use a MIME library for your programming language to do this. Pass the resulting MIME string as message parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ff87b61-d4d9-4b16-9fb8-220e5a564129"
            }
          ]
        },
        {
          "id": "29c1d02d-8502-47a1-a601-ec56654294b8",
          "name": "putRoutes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "routes/:id"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "expression",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "priority",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a given route by ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d6ab3c9-2ce1-4826-a582-2ff98582b409"
            }
          ]
        }
      ]
    },
    {
      "name": "Send",
      "item": [
        {
          "id": "2161ffe8-fe7d-43b4-be25-103be118df8c",
          "name": "postMessages",
          "request": {
            "url": "http://api.mailgun.net/v2/messages/?attachment=%7B%7D&bcc=%7B%7D&cc=%7B%7D&from=%7B%7D&h:X-My-Header=%7B%7D&html=%7B%7D&inline=%7B%7D&o:campaign=%7B%7D&o:deliverytime=%7B%7D&o:dkim=%7B%7D&o:tag=%7B%7D&o:testmode=%7B%7D&o:tracking=%7B%7D&o:tracking-clicks=%7B%7D&o:tracking-opens=%7B%7D&subject=%7B%7D&text=%7B%7D&to=%7B%7D&v:my-var=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a message by assembling it from the components. Note that you can specify most parameters multiple times, HTTP supports this out of the box. This makes sense for parameters like cc, to or attachment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f81a7b10-44be-4ac9-87fa-4488e9d92a5c"
            }
          ]
        }
      ]
    },
    {
      "name": "Message",
      "item": [
        {
          "id": "6e960e42-16a7-4b05-ba14-de0afbcfd689",
          "name": "getMessages",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "messages/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0635efb5-f026-4375-9a56-b4a621be7bb8"
            }
          ]
        }
      ]
    },
    {
      "name": "Routes",
      "item": [
        {
          "id": "e93bd97c-eda9-4c09-b20a-2bc2d0924709",
          "name": "getRoutes",
          "request": {
            "url": "http://api.mailgun.net/v2/routes/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches the list of routes. Note that routes are defined globally, per account, not per domain as most of other API calls."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1ff4929-8200-4378-affa-013d679ebff5"
            }
          ]
        }
      ]
    },
    {
      "name": "Route",
      "item": [
        {
          "id": "a75b298c-0c03-4c44-878a-01551f4dbd93",
          "name": "postRoutes",
          "request": {
            "url": "http://api.mailgun.net/v2/routes/?action=%7B%7D&description=%7B%7D&expression=%7B%7D&priority=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new route."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa145a83-8733-4eb3-92f1-ea9e21a02fe8"
            }
          ]
        },
        {
          "id": "978577eb-fcba-4eb0-95e3-9be7b769945a",
          "name": "getRoutes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "routes/:id"
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
            "description": "Returns a single route object based on its ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b8588cc-5e6b-421c-9a6c-9da869456135"
            }
          ]
        },
        {
          "id": "6d07f369-6f11-4faa-8314-ad855f6a3618",
          "name": "deleteRoutes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "routes/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a route based on the id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "296252fb-851a-4344-9f1a-53deaf5303cd"
            }
          ]
        }
      ]
    },
    {
      "name": "Stats",
      "item": [
        {
          "id": "0c3948d8-521c-4df3-a9d3-75069612e4a1",
          "name": "getStats",
          "request": {
            "url": "http://api.mailgun.net/v2/stats/?event=%7B%7D&limit=%7B%7D&skip=%7B%7D&start-date=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of event stat items. Each record represents counts for one event per one day."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "969cd035-0272-4f05-962f-9157da3d0bf7"
            }
          ]
        }
      ]
    },
    {
      "name": "Tag",
      "item": [
        {
          "id": "279f8edb-5ea2-43f7-a171-6f4d43ce934b",
          "name": "deleteTagsTag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "tags/:tag"
              ],
              "variable": [
                {
                  "id": "tag",
                  "value": "tag",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes all counters for particular tag and the tag itself."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "403a3e5b-1633-41d0-b18b-a190e2521914"
            }
          ]
        }
      ]
    }
  ]
}