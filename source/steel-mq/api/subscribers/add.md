---
layout: steelmq
title: Steel-MQ API Add Subscriber to Message Queue
---

Add Subscriber to Message Queue
===============================

```
POST /projects/{Project ID}/queues/{Queue ID}/subscribers
```

### Request

``` json
{
    "subscriber": {
        "url": "http://some.subscriber.com/steel_mq_hook",
        "headers": {
            "Content-Type": [
                "application/json"
            ],
            "X-Custom": [
                "foo",
                "bar"
            ]
        }
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

Requires role: ```subscribe```
