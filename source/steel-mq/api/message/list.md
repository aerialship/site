---
layout: steelmq
title: Steel-MQ API Get Messages from Queue
---

Get Messages from Queue
=======================

```
GET /projects/{Project ID}/queues/{Queue ID}/messages
```

### URL Parameters

* limit - optional, integer, defaults to 1, maximum is 100. Note that you might not receive all requested messages, but only those available at the moment of the request
* timeout - optional, integer, defaults to message queue timeout which defaults to 60, number of seconds after which message will be placed back on the queue, unless deleted or timeout expanded
* delete - optional, boolean, defaults to false, if true message will be deleted immediately on this request. Be careful and use this only if losing a message is ok

### Response

``` json
{
    "messages": [
        {
            "id": 123,
            "body": "Body message string",
            "timeout": 60,
            "retries_remaining": 3
        }
    ]
}
```