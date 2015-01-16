---
layout: steelmq
title: Steel-MQ API Message Queue Update
---

Update Message Queue
====================

```
POST /projects/{Project ID}/queues/{Queue ID}
```

### Body Parameters

* title - required, string, name of the queue to create
* push_type - optional, ```pull```, ```unicast```, or ```multicast```, defaults to ```pull```
* retries - optional, integer, defaults to 5, number of time to retry to deliver the message
* retries_delay - optional, integer, defaults to 600, number of seconds to wait before next retry
* error_queue - optional, integer, defults to null, queue id to put messages to when message was not delivered after all retries

### Request

``` json
{
    "queue": {
        "title": "New Queue Name",
        "push_type": "unicast",
        "retries": 5,
        "retries_delay": 600,
        "error_queue": 678,
        "timeout": 60,
        "delay": 0,
        "expires_in": 604800
    }
}
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
    "error_queue": 678
}
```

Requires role: ```queue```
