# Technical Writing

## JIRA Task Statuses

Work with documentation tasks in DOC container in JIRA.

| Status        | Description  |
|---|---|
| **Backlog**       | Use **Backlog** status for new tasks  |
| **To Do**         | Use **To Do** status if you are going to work on the task in the upcoming week  |
| **In Progress**   | Use **In Progress** status on active tasks  |
| **Review**        | Use **Review** status on tasks in the process of review with customer or cross-review in writer's team  |
| **Done**          | Use **Done** status on completed tasks  |
| *Flag (Paused)* | Use *Flag* feature in Jira if all work on task is paused  |

## API Documentation 

This is an example of API documentation. You can find full version [here](https://docs.bnmap.pro/api-docs/api-methods/api-get-prices) (available only in Russian).

### GET Prices

Use **GET Prices** method to acquire prices data from API bnMap.pro service.

#### Parameters

|Name  |Required   |Description   |
|---|---|---|
|pbi   |Yes   |Personal authorization token   |

#### Request Example

```bash
curl -X 'GET' \
  'https://api.bndev.it/cmap/analytics.json?act=pbi-prices&test=true&pbi=TOKEN' \
  -H 'accept: application/json'
```

#### Response Example

```json
{
  "status": "ok",
  "content": [ hidden for security reasons
  ],
  "auth": true
}
```