{
  "info": {
    "name": "Mailgun API Routes",
    "_postman_id": "a74cf6c9-d9d1-481e-b872-cb0c2a008099",
    "description": "Fetches the list of routes. Note that routes are defined globally, per account, not per domain as most of other API calls.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bounces",
      "item": [
        {
          "id": "f9b1b945-aba1-4bae-86bd-be8ae41cf55b",
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
              "id": "182b42aa-9d8f-4162-89f5-0f551564928c"
            }
          ]
        }
      ]
    },
    {
      "name": "Bounce",
      "item": [
        {
          "id": "55133dd6-82ab-4c08-9de5-b7bc5cfcd5af",
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
              "id": "c935b5e5-871a-4f74-b4de-c545f296e0a7"
            }
          ]
        },
        {
          "id": "f6551d70-d933-4243-87eb-78c74cb40cb0",
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
              "id": "8df8159c-711e-4db2-b5f9-29afac1f3ae1"
            }
          ]
        },
        {
          "id": "fc8e2fa3-1acc-42dc-aff8-dd1d6110633c",
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
              "id": "1b6b19ea-6c00-4888-9d7b-49d038f72f30"
            }
          ]
        }
      ]
    },
    {
      "name": "Complaints",
      "item": [
        {
          "id": "6cd379b2-957c-457c-bfd7-786fc8163ce3",
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
              "id": "89cf0c8e-36d7-4071-b095-d450734d0927"
            }
          ]
        }
      ]
    },
    {
      "name": "Complaint",
      "item": [
        {
          "id": "605c5054-80f3-407b-8f94-e5b2cb930448",
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
              "id": "1cc13d47-c503-4197-a0da-d4ffeb2212e3"
            }
          ]
        },
        {
          "id": "6fd8a6ed-7026-40c1-bbc7-1c749b2dbd03",
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
              "id": "ede0faa1-fbd2-484d-b66a-9d240e90f58b"
            }
          ]
        },
        {
          "id": "dac15da0-93ee-41cd-bb94-72e2d2c81739",
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
              "id": "9687960b-bf78-4f1a-8635-45dde44d7573"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "d8e1f4f8-c833-44e6-8bc9-aea46302c745",
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
              "id": "f5577208-3652-485b-8fed-f5e18806dd84"
            }
          ]
        },
        {
          "id": "9e658c8f-ec7f-4aac-bdb3-9c1c5f3540eb",
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
              "id": "95333372-cd33-4948-b1c3-415ed93a5551"
            }
          ]
        },
        {
          "id": "f9f423b4-bc79-4104-84bc-d7e46c3411c8",
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
              "id": "31652b2a-e93c-4435-b4a9-b96c7ffbcd83"
            }
          ]
        },
        {
          "id": "772099c4-b06e-4c77-9a6a-2cbd2a3668c1",
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
              "id": "8b10253b-573d-4bee-a98b-c06d2e40896a"
            }
          ]
        },
        {
          "id": "c32b57bb-9bc8-45b3-8390-94ebc1867f01",
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
              "id": "bc69f42e-e279-487d-a26b-4bd7793ed736"
            }
          ]
        },
        {
          "id": "44f2fd59-256e-4578-94c0-8b7491fab513",
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
              "id": "3ca5b198-7ac0-4f3f-aa24-8f0dd838ff70"
            }
          ]
        },
        {
          "id": "0f180f43-a1c0-435c-8203-05676f11abe0",
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
              "id": "7e7d5ab8-36c8-40fe-b66f-c33c911feabb"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "05eac045-ebb6-4c43-abe2-7d76eed912da",
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
              "id": "1af16e74-eb79-48af-ba9c-2cb18028b5c3"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "efc62160-5740-40fe-ab6c-9a0aabf7e715",
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
              "id": "cca3d400-979b-4ca4-86e8-9e43bc38ffb5"
            }
          ]
        }
      ]
    },
    {
      "name": "Send",
      "item": [
        {
          "id": "366258ef-28ef-429b-916b-352cf2431f18",
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
              "id": "64970588-4f10-4e21-bc81-885a59d2d591"
            }
          ]
        }
      ]
    },
    {
      "name": "Message",
      "item": [
        {
          "id": "6abcee62-ce66-4f82-902f-d66a42826dfb",
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
              "id": "0e6e39d5-76be-40c1-867f-472038519f13"
            }
          ]
        }
      ]
    },
    {
      "name": "Routes",
      "item": [
        {
          "id": "29e03c9c-6de5-4ee2-9ac8-8882176029f4",
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
              "id": "e8a9e0fe-ceac-4e02-99f1-3ac713ee615e"
            }
          ]
        }
      ]
    }
  ]
}