---
layout: steelmq
title: Steel-MQ API Add Messages to Queue
---

Add Messages to Queue
=====================

```
POST /projects/{Project ID}/queues/{Queue ID}/messages
```

### Request

``` json
{
    "messages": [
        {
            "body": "Message string body",
            "delay": 0,
            "retries": 3
        }
    ]
}
```
