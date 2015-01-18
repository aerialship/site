---
layout: asjs
title: Trigger event - AS-JS Example
---

# trigger

## Example

<div class="row">
    <div class="col-md-3">
        <button type="button"
            data-as='{
                "click": {
                    "trigger": {
                        "event": "something"
                    }
                }
            }'
        >Trigger something</button>
    </div>

    <div class="col-md-3"
        data-as='{
            "something": {
                "html": {
                    "result": "<p>Lorem ipsum dolores sit</p>",
                    "target": "#target"
                }
            }
        }'
    >Event 'something' makes me render 'lorem ipsum' in #target</div>

    <div id="target" class="col-md-3">...</div>
</div>

<div class="mt-30"></div>

## Source

``` html
<button type="button"
    data-as='{
        "click": {
            "trigger": {
                "event": "something"
            }
        }
    }'
>Trigger something</button>

<div
    data-as='{
        "something": {
            "html": {
                "result": "<p>Lorem ipsum dolores sit</p>",
                "target": "#target"
            }
        }
    }'
>Event 'something' makes me render 'lorem ipsum' in #target</div>

<div id="target">...</div>
```
