---
layout: asjs
title: Load - AS-JS Example
---

# Load

## Example

<div class="row">
    <div class="col-md-6">
        <button type="button"
            data-as='{
                "click": {
                    "load": {
                        "url": "./data/partial_content.html",
                        "block": true,
                        "blockOptions": {
                            "message": "<h2>Custom loading message</h2>"
                        },
                        "success": {
                            "html": {
                                "target": "#target"
                            }
                        }
                    }
                }
            }'
        >Load content</button>
    </div>

    <div id="target" class="col-md-6">
        it will be loaded here...
    </div>
</div>

<div class="mt-30"></div>

## Source

``` html
<button type="button"
    data-as='{
        "click": {
            "load": {
                "url": "partial_content.html",
                "block": true,
                "blockOptions": {
                    "message": "<h2>Custom loading message</h2>"
                },
                "success": {
                    "html": {
                        "target": "#target"
                    }
                }
            }
        }
    }'
>Load content</button>

<div id="target">
    it will be loaded here...
</div>
```
