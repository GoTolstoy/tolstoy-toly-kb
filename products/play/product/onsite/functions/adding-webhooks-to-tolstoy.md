## Adding Webhooks to Tolstoy

Are you interested in sending your Tolstoy data directly to a web app or URL? Follow this guide to learn how to set up webhooks to receive notifications when a viewer interacts with your Tolstoy!

### Getting Your API Token

First, get your API Token.

### Configuring a Webhook Using REST API

Paste your token in the request Authorization Header as `Bearer YOUR_API_TOKEN`.

**Base URL:**

```
https://api.gotolstoy.com
```

**Methods and Routes:**

| Method | Route              | Description                |
|--------|--------------------|----------------------------|
| GET    | /webhooks/         | List subscriptions         |
| POST   | /webhooks/         | Create a subscription      |
| GET    | /webhooks/:id/     | Get a subscription         |
| PUT    | /webhooks/:id/     | Update a subscription      |
| DELETE | /webhooks/:id/     | Delete a subscription      |

### Supported Events

- `response_summary` - Get a summary of a viewer session in Tolstoy.
- `collected_info` - Get a summary of a viewer session in Tolstoy only if there was a lead form submitted.

### Examples

**Request to Add a Webhook:**

```sh
curl --location --request POST 'https://api.gotolstoy.com/webhooks/' \
--header 'Authorization: Bearer YOUR_API_TOKEN' \
--header 'Content-Type: application/json' \
--data-raw '{
""url"": ""https://YOUR_URL/"",
""event"": ""response_summary""
}'
```

**Request to See Your Defined Webhooks:**

```sh
curl --location --request GET 'https://api.gotolstoy.com/webhooks/' \
--header 'Authorization: Bearer YOUR_API_TOKEN'
```

### Response Summary Event Example

```json
{
  ""subscribers"": [],
  ""notificationLevel"": 4,
  ""user"": ""Anonymous"",
  ""playlist"": ""Tolstoy #5"",
  ""publishId"": ""zgo4t6htijvzz"",
  ""timestamp"": ""2021-03-11T11:52:19.968Z"",
  ""accountId"": ""43a7bd93-c302-4c18-93bc-d7151c586336"",
  ""accountEmail"": ""nimrod.popper@gmail.com"",
  ""anonymousId"": ""ab63ae8f-1c96-4fc6-baf3-a9c3b9ad0eab"",
  ""collectedInfo"": {
    ""email"": ""newuser@test.com"",
    ""name"": ""newuser"",
    ""phone"": ""123123""
  },
  ""events"": [
    {
      ""videoName"": ""Question 1.mov"",
      ""eventName"": ""pageView"",
      ""question"": """",
      ""timestamp"": ""2021-03-11T11:52:17.383Z""
    },
    {
      ""videoName"": ""Question 1.mov"",
      ""eventName"": ""sessionStart"",
      ""question"": """",
      ""timestamp"": ""2021-03-11T11:52:18.253Z""
    },
    {
      ""videoName"": ""Question 1.mov"",
      ""text"": ""heyy"",
      ""eventName"": ""clickCta"",
      ""question"": """",
      ""timestamp"": ""2021-03-11T11:52:19.968Z""
    },
    {
      ""videoName"": ""1 intro.mp4"",
      ""text"": ""test"",
      ""eventName"": ""clickCta"",
      ""question"": """",
      ""timestamp"": ""2021-03-11T11:52:22.703Z""
    },
    {
      ""videoName"": ""1 intro.mp4"",
      ""eventName"": ""sessionEnd"",
      ""question"": """",
      ""timestamp"": ""2021-03-11T11:52:22.713Z""
    }
  ],
  ""sessionTime"": ""93""
}
```