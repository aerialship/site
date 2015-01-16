---
layout: steelmq
title: Steel-MQ API Release Message back to Queue
---

Release Message back to Queue
=============================

```
POST /projects/{Project ID}/queues/{Queue ID}/messages/{Message ID}/release
```

### Body Parameters

* delay - optional, integer, defaults to 0, number of seconds until message becomes available on the queue

### Request

``` json
{
    "delay": 60
}
```

### Response

``` json
{
    "success": true
}
```
