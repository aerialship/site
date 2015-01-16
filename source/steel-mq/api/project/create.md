---
layout: steelmq
title: Steel-MQ API Project Create
---

Create Project
==============

```
POST /projects
```

### Request

``` json
{
    "project": {
        "title": "Project name"
    }
}
```

### Response

``` json
{
    "id": 123,
    "success": true
}
```
```