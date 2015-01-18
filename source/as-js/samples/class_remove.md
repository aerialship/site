---
layout: asjs
title: Class remove - AS-JS Example
---

# class.remove

## Example

<div class="row mt-30">
    <div class="col-md-6">
        <button type="button"
            data-as='{
                "click": {
                    "class.remove": {
                        "target": "#second",
                        "class": "asjs-selected"
                    }
                }
            }'
        >Add Class 'selected' to #second</button>
    </div>
    <div class="col-md-6">
        <ul>
            <li id="first">First</li>
            <li id="second" class="asjs-selected">Second</li>
            <li id="third">Third</li>
        </ul>
    </div>
</div>

## Source

``` html
<button type="button"
    data-as='{
        "click": {
            "class.remove": {
                "target": "#second",
                "class": "asjs-selected"
            }
        }
    }'
>Add Class 'selected' to #second</button>

<ul>
    <li id="first">First</li>
    <li id="second" class="asjs-selected">Second</li>
    <li id="third">Third</li>
</ul>

```