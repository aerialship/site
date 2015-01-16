---
layout: steelmq
title: Steel-MQ API Get Message by ID
---

Get Message by ID
=================

```
GET /projects/{Project ID}/queues/{Queue ID}/messages/{Message ID}
```

### Response

``` json
{
    "id": 123,
    "body": "Message Body String",
    "timeout": 60,
    "created_at": "2014-01-01 12:25:36Z",
    "completed_at": "2014-01-01 14:18:54Z"
}
```
