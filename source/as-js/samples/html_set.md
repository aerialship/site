---
layout: asjs
title: Html set - AS-JS Example
---

# html set

## Example

<div class="row">
    <div class="col-md-6">
        <button type="button"
            data-as='{
                "click": {
                    "html": {
                        "result": "<p>Lorem ipsum dolores sit</p>",
                        "target": "#target"
                    }
                }
            }'
        >Set content</button>
    </div>

    <div id="target" class="col-md-6">
        it will be put here...
    </div>
</div>

<div class="mt-30"></div>

## Source

``` html
<button type="button"
    data-as='{
        "click": {
            "html": {
                "result": "<p>Lorem ipsum dolores sit</p>",
                "target": "#target"
            }
        }
    }'
>Set content</button>

<div id="target">
    it will be added here...
</div>
```
