---
layout: steelmq
title: Steel-MQ API List Message Queue Subscribers
---

List Message Queue Subscribers
==============================

```
GET /projects/{Project ID}/queues/{Queue ID}/subscribers
```

### URL Parameters

* limit - optional, integer, defaults to 100, number of subscribers to return
* offset - optional, integer, defaults to 0

### Response

``` json
[
    {
        "id": 123,
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
]
```