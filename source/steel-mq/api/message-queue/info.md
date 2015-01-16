---
layout: steelmq
title: Steel-MQ API Message Queue Info
---

Get Message Queue Info
======================

```
GET /projects/{Project ID}/queues/{Queue ID}
```

### Response

``` json
{
    "id": 123,
    "title": "Queue name",
    "project_id": 456,
    "push_type": "unicast",
    "retries": 5,
    "retries_delay": 600,
    "error_queue": 678,
    "timeout": 60,
    "delay": 0,
    "expires_in": 604800
    "size": 12
}
```
