# Janus

Janus will read your database DLL, do a bit of prompt engineering, and then automatically generate SQL queries that answer your question. Janus is designed to do basic descriptive analytics - which broadly means it'll help you summarize the past and find counts, trends, etc. The intention of this tool is to automate the first step of most data analytics workflows, the development of ad-hoc dashboards for monitoring and visualization, and to reduce the load on teams that get asked analytics questions in Slack. 

### Components

#### Web Server
WIP

Endpoints:
- POST /api/prompt 

```sh
curl "http://localhost:3000/api/prompt" -D '{ "name": "test-prompt", "connectionURL": "...", "filters": { "schema": "...", "includeTables": [], "excludeTables": [] }  }'
```

- GET /api/answer

```sh
curl "http://localhost:3000/api/answer?prompt=text-prompt"
```
