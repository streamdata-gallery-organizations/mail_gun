{
  "info": {
    "name": "Mailgun API Stats",
    "_postman_id": "2c2f444e-0107-4012-8615-9c52f0f1fdba",
    "description": "Returns a list of event stat items. Each record represents counts for one event per one day.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bounces",
      "item": [
        {
          "id": "ff758a6d-89c1-46e5-923b-a3492655c06e",
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
              "id": "81aafbc4-2ea1-4852-bebc-52457b9cd590"
            }
          ]
        }
      ]
    },
    {
      "name": "Bounce",
      "item": [
        {
          "id": "2250e257-0228-47d5-98e9-6c4cbda2c422",
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
              "id": "a7ca7a0d-3a0f-48b2-8c91-557b29eed3c5"
            }
          ]
        },
        {
          "id": "161d5ce9-cfa7-40eb-b02f-1a29ada4ad1f",
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
              "id": "563348b8-44cf-4fe1-af95-3ef7305f2ecc"
            }
          ]
        },
        {
          "id": "55c019b5-4d7d-485e-85f3-76a282f51873",
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
              "id": "3b7f0421-ee72-4251-9a9f-25c969050fd5"
            }
          ]
        }
      ]
    },
    {
      "name": "Complaints",
      "item": [
        {
          "id": "f4922a15-a623-4b3a-b751-83720daad00f",
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
              "id": "14c79d93-b12e-4a97-a713-cae47d26b03a"
            }
          ]
        }
      ]
    },
    {
      "name": "Complaint",
      "item": [
        {
          "id": "1ac0cee2-9674-4e26-ac99-aad7caaab0d8",
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
              "id": "01048e14-8d08-4dfc-9acf-e169400445fc"
            }
          ]
        },
        {
          "id": "1869dea5-44e7-43d9-bd01-f0b7cb5631fa",
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
              "id": "7887ef55-53da-4639-bb8a-a256015c68c0"
            }
          ]
        },
        {
          "id": "07ce1663-6e62-4062-9842-590baa9f2388",
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
              "id": "5f6f78cc-fde1-476f-9ced-aa8f59c42707"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "1d1d7ae6-79ef-4502-82ed-ae1e1e8f99d4",
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
              "id": "9fb380d4-b1e6-4c8a-b864-982a410393f6"
            }
          ]
        },
        {
          "id": "9a3378d4-5c95-4558-82fa-769d5f61e8d8",
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
              "id": "d0760ea2-22b7-4a0c-b8a4-26f75f458c31"
            }
          ]
        },
        {
          "id": "77e1aa02-19a3-4aef-9d5e-71c455c7294b",
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
              "id": "62e7a18e-1852-427f-bafd-16d03761a896"
            }
          ]
        },
        {
          "id": "3b78346e-21ac-402b-8ae8-5ca65b9fee09",
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
              "id": "a3f9cdd0-25f0-426b-a039-a2e2466ad91f"
            }
          ]
        },
        {
          "id": "94858b84-6674-4ecd-9812-671c732a8f26",
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
              "id": "5f1dcefa-fd1f-4bb7-8855-2bba5de411ae"
            }
          ]
        },
        {
          "id": "edcb3e8a-3f2e-4cf9-9eca-6792e0980fdc",
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
              "id": "fdd30a8b-acbd-4903-8f57-ab03c783211b"
            }
          ]
        },
        {
          "id": "adbc5dc5-0a16-4f70-bff4-41c34971e597",
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
              "id": "ce730d32-9580-432e-9413-bd8cb8870613"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "d7f88c2c-b51c-437a-b4ce-c52cee3b17cc",
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
              "id": "3be551b0-1d1d-4c96-8091-7c36730349c6"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "e2bee8a3-8690-4b02-b5be-1e925da7aed3",
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
              "id": "a16eee78-6634-44c9-bd2b-98b8a108a063"
            }
          ]
        },
        {
          "id": "b19b9f65-d80c-4579-8855-363a799809bd",
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
              "id": "e6de62d0-4fbe-4319-b6ba-5fdc52c5b493"
            }
          ]
        }
      ]
    },
    {
      "name": "Send",
      "item": [
        {
          "id": "80c3dffd-5623-46b3-ac6e-56fb033e6c81",
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
              "id": "36f8cd7a-ab84-445e-994e-7f96b4fb6f5a"
            }
          ]
        }
      ]
    },
    {
      "name": "Message",
      "item": [
        {
          "id": "3c6f0c95-4cad-482c-9e62-7406d1a9a0ef",
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
              "id": "ac8b34a0-b00e-4056-b640-e573b46e70f9"
            }
          ]
        }
      ]
    },
    {
      "name": "Routes",
      "item": [
        {
          "id": "4afdacc1-b9f8-4fe3-90eb-094d3cc4e597",
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
              "id": "56e154cb-1536-4476-a632-07b1b9271206"
            }
          ]
        }
      ]
    },
    {
      "name": "Route",
      "item": [
        {
          "id": "d9f8bef9-fdfe-45ac-a74d-bd70e776c857",
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
              "id": "846bf75f-0299-439f-8df8-c52bfc064e17"
            }
          ]
        },
        {
          "id": "6fd13adf-564e-4696-87d0-5ca23250a108",
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
              "id": "abf092f6-7fe3-4716-98c1-e0afe86d5eaf"
            }
          ]
        },
        {
          "id": "1f04657c-7c8f-4e4d-820a-8f97729769c4",
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
              "id": "b092cf4f-c88c-4b28-bff8-6e97c9bf60b1"
            }
          ]
        }
      ]
    },
    {
      "name": "Stats",
      "item": [
        {
          "id": "09b1ae32-a2b2-4e7b-905d-7a02901040b6",
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
              "id": "fd0cf1bc-2d75-40cc-a6d3-7c284f6ac234"
            }
          ]
        }
      ]
    }
  ]
}