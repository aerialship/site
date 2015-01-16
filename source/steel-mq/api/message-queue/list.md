---
layout: steelmq
title: Steel-MQ API Message Queue List
---

List Message Queues
===================

```
GET /projects/{Project ID}/queues
```

### URL Parameters

* limit - optional, integer, defaults to 100, number of queues to return
* offset - optional, integer, defaults to 0


### Response

``` json
[
    {
        "id": 123,
        "title": "Queue name",
        "project_id": 456,
        "push_type": "unicast",
        "retries": 5,
        "retries_delay": 600,
        "error_queue": 678
    }
]
```
