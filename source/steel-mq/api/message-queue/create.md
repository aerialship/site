---
layout: steelmq
title: Steel-MQ API Message Queue Create
---

Create Message Queue
====================

```
POST /projects/{Project ID}/queues
```

### Body Parameters

* title - required, string, name of the queue to create
* push_type - optional, ```pull```, ```unicast```, or ```multicast```, defaults to ```pull```
* retries - optional, integer, defaults to 5, number of time to retry to deliver the message
* retries_delay - optional, integer, defaults to 600, number of seconds to wait before next retry
* error_queue - optional, integer, defaults to null, queue id to put messages to when message was not delivered after all retries
* timeout - optional, integer, defaults to 60, number of seconds taken message will timeout and put back on queue, can be overridden when creating message
* delay - optional, integer, defaults to 0, number of seconds until created messages gets available on the queue, can be overridden when creating message
* expires_in - optional, integer, defaults to 604800 (7 days), number of seconds to keep messages in the queue before they are deleted, can be overridden when creating message

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
