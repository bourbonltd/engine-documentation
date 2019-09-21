# Overview

## Widgets

- [Basics](widgets/basics.md)
- [App Bars](widgets/app-bars.md)
- [Dynamic Lists/Grids](widgets/dynamic-lists-grids.md)
- [Fixed List/Grids](widgets/fixed-lists-grids.md)

## Configurations

The configuration is used to define brand details such as typography, colours, padding, etc. It also references the templates and their version.

Versioning allows you to switch the base configuration, templates and data resources on-demand without changing anything within the native app.

[Example](../examples/Bird/configurations/Demo-1.json) configuration.

## Templates

Templates define what the view should render, this can be a simple list showing names and avatars or a full blown user profile page with posts, recent activities etc.

The most important items within a template are Components & Data

[Example](../examples/Bird/templates/Home-1.json) template.

## Data Definitions

Data definitions serve as template data sources, they provide templates with access to content from other JSON APIs.

```json
{
  "version": 1,
  "engineVersion": 1,
  "name": "getTopics",
  "method": "GET",
  "endpoint": "http://api.bourbon.sh/news/{userId}/topics",
  "requestHeaders": {
    "Authorization": "Bearer {jwtToken}"
  },
  "requestBody": {},
  "caching": {
    "age": 3600,
    "key": ["{userId}", "topics"]
  }
}
```

[Example](../examples/Bird/data/getActivity-1.json) data definition.