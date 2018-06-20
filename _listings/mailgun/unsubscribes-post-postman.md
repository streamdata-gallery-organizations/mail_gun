{
  "info": {
    "name": "Mailgun API Add to unsubscribe list.",
    "_postman_id": "91f1c1e9-0b09-4980-b897-8f415d07d55a",
    "description": "Adds address to unsubscribed table.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bounces",
      "item": [
        {
          "id": "9d2b8222-1444-4f3f-b31e-4eda490073e8",
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
              "id": "24c30b8c-365b-4f21-82f5-3625509f2f9f"
            }
          ]
        }
      ]
    },
    {
      "name": "Bounce",
      "item": [
        {
          "id": "e3640694-87ae-437d-9f84-d58e3a9bb10c",
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
              "id": "0cebdbd7-26d5-42e5-a75e-c26502147f81"
            }
          ]
        },
        {
          "id": "fb584b95-7fb1-42a9-9ce0-2a82a5174a1a",
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
              "id": "f3dcc41e-a895-4087-a204-b28386bf5fa0"
            }
          ]
        },
        {
          "id": "d7062b74-6d57-4fa5-9774-eebb0f3c3b88",
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
              "id": "3fb9cdef-bf32-41ef-8f04-8dd87659cc41"
            }
          ]
        }
      ]
    },
    {
      "name": "Complaints",
      "item": [
        {
          "id": "7243994b-0e58-4596-93d8-72d051bb5c82",
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
              "id": "759ccf4e-4167-43a3-b659-d949fb0e4f08"
            }
          ]
        }
      ]
    },
    {
      "name": "Complaint",
      "item": [
        {
          "id": "759d9eda-2d46-46a3-ac98-42d2c0d56ce8",
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
              "id": "aa379469-1048-4aff-81bd-952df8b7f7f2"
            }
          ]
        },
        {
          "id": "5a03e26b-937f-44da-9474-51c80018d589",
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
              "id": "8e1ca35e-9ac5-4984-9f84-0c3d8c89c9ad"
            }
          ]
        },
        {
          "id": "071fb1be-51f8-47a7-9196-83139352c7e6",
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
              "id": "a355cc8f-0279-409c-bdcd-864212106456"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "add93955-6d48-4488-9aab-85c81c9b160f",
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
              "id": "a29c021f-b380-4184-a0f1-445056d923c6"
            }
          ]
        },
        {
          "id": "435fb4f4-91cb-400c-8d2c-51cfa43063c3",
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
              "id": "d19da7a6-317a-4b89-85da-69392076e812"
            }
          ]
        },
        {
          "id": "e3392a6b-906b-4ebe-af5a-02ce18dd4ebb",
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
              "id": "112f607a-07be-4afd-9d5d-64fc4a6ab738"
            }
          ]
        },
        {
          "id": "60792926-2606-4eff-99e7-72840f3d100e",
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
              "id": "e1cf95ba-7144-46c5-ada8-e1ea7fdf42af"
            }
          ]
        },
        {
          "id": "700acdcd-932a-43da-b303-d7bb4e6892d1",
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
              "id": "4dca53be-8054-4e06-beb3-b7cac618b6bb"
            }
          ]
        },
        {
          "id": "e9ba6a15-f168-4e89-9850-41501e7a3878",
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
              "id": "0ee8dbde-c3c0-46bb-b5fd-9c8ff72eca08"
            }
          ]
        },
        {
          "id": "34566030-7ad5-491c-a70c-14d6c57b6072",
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
              "id": "7d5680a2-cbb3-40c4-9106-6de628e98657"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "44095861-069d-462a-b50c-3fa9780a257b",
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
              "id": "f6020092-5490-47f4-bf83-e1b89ee59ece"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "7dc15764-98cc-4301-99f0-c653bdf94777",
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
              "id": "a76d17c2-e3a7-41a2-9cbe-936f28a751d0"
            }
          ]
        },
        {
          "id": "f65e5cbd-5b4a-471d-acb6-4c217055ce9f",
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
              "id": "3499c648-425f-40ee-b5f3-77c62fb3643c"
            }
          ]
        }
      ]
    },
    {
      "name": "Send",
      "item": [
        {
          "id": "6d55276e-b979-4d8a-ae57-8db4c2f069e7",
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
              "id": "e795c693-d0ac-4435-9102-c9787fba5468"
            }
          ]
        }
      ]
    },
    {
      "name": "Message",
      "item": [
        {
          "id": "0a12fb94-09ce-4699-a514-44f702644cec",
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
              "id": "bd94bdd9-70aa-40dd-840b-7b0f84f73aef"
            }
          ]
        }
      ]
    },
    {
      "name": "Routes",
      "item": [
        {
          "id": "a2ce91ec-8a1d-4bb1-b60c-5e7659beb8fd",
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
              "id": "f1ea6929-8a96-419e-aded-55247cb5f794"
            }
          ]
        }
      ]
    },
    {
      "name": "Route",
      "item": [
        {
          "id": "6046ddad-fd44-4946-9241-1e68b253bfb1",
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
              "id": "34637138-0522-445f-82ae-1fa932b49170"
            }
          ]
        },
        {
          "id": "2fcdddaf-8734-4a02-8529-f017efb47739",
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
              "id": "fe84db18-e466-4519-ada7-8ec38c55774d"
            }
          ]
        },
        {
          "id": "7620908b-e4d8-400b-9124-df6027b1cfcc",
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
              "id": "8bd62588-fd85-4c9d-b196-8d07292f75f1"
            }
          ]
        }
      ]
    },
    {
      "name": "Stats",
      "item": [
        {
          "id": "fc053d52-a1db-4373-a180-468cae1d8caf",
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
              "id": "69ab79f9-3731-4a0a-be6b-1c39ffd7d19f"
            }
          ]
        }
      ]
    },
    {
      "name": "Tag",
      "item": [
        {
          "id": "50631116-85ef-4b92-865d-90b5ae3ae99d",
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
              "id": "2081b64b-6bfc-45c8-940b-6fb9a4dd7ab5"
            }
          ]
        }
      ]
    },
    {
      "name": "Unsubscribes",
      "item": [
        {
          "id": "85282fc2-236d-4049-b580-6998f4880ba2",
          "name": "getUnsubscribes",
          "request": {
            "url": "http://api.mailgun.net/v2/unsubscribes/?limit=%7B%7D&skip=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API allows you to programmatically download the list of recipients who have unsubscribed from your emails."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff58f99e-cdd8-4c11-adcd-00b9fda6860e"
            }
          ]
        }
      ]
    },
    {
      "name": "To",
      "item": [
        {
          "id": "c8959b6b-2c61-4ba8-a960-725b9fc0ffc8",
          "name": "postUnsubscribes",
          "request": {
            "url": "http://api.mailgun.net/v2/unsubscribes/?address=%7B%7D&tag=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds address to unsubscribed table."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c13d930-6916-4cf6-8afb-4991aa7b9c18"
            }
          ]
        }
      ]
    }
  ]
}