---
layout: asjs
title: Class toggle radio - AS-JS Example
---

# class.toggle

## Example

<div class="row mt-30">
    <div class="col-md-6">

        <button type="button"
            data-as='{
                "click": {
                    "class.toggle": {
                        "target": "#a",
                        "class": "asjs-selected",
                        "parent": true
                    }
                }
            }'
        >A</button>
        <button type="button"
            data-as='{
                "click": {
                    "class.toggle": {
                        "target": "#b",
                        "class": "asjs-selected",
                        "parent": true
                    }
                }
            }'
        >B</button>
        <button type="button"
            data-as='{
                "click": {
                    "class.toggle": {
                        "target": "#c",
                        "class": "asjs-selected",
                        "parent": true
                    }
                }
            }'
        >C</button>

    </div>
    <div class="col-md-6">
        <ul>
            <li id="a">First</li>
            <li id="b">Second</li>
            <li id="c">Third</li>
        </ul>
    </div>
</div>

## Source

```
<button type="button"                                       <ul>
    data-as='{                                                  <li id="a">First</li>
        "click": {                                              <li id="b">Second</li>
            "class.toggle": {                                   <li id="c">Third</li>
                "target": "#a",                             </ul>
                "class": "asjs-selected",
                "parent": true
            }
        }
    }'
>A</button>
<button type="button"
    data-as='{
        "click": {
            "class.toggle": {
                "target": "#b",
                "class": "asjs-selected",
                "parent": true
            }
        }
    }'
>B</button>
<button type="button"
    data-as='{
        "click": {
            "class.toggle": {
                "target": "#c",
                "class": "asjs-selected",
                "parent": true
            }
        }
    }'
>C</button>
```
