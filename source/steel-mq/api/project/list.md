---
layout: steelmq
title: Steel-MQ API Project List
---

List Projects
=============

```
GET /projects
```

### Response

``` json
[
    {
        "id": 123,
        "title": "Project name",
        "roles": ["owner", "default", "queue", "subscribe", "share"]
    }
]
```
