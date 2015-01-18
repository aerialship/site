---
layout: asjs
title: Bootstrap Modal Load (short way) - AS-JS Example
---

# Bootstrap Modal Load (short way)

This example demonstrates loading of remove bootstrap modal content and showing it once loaded. It's a convenient
shortcut for the full implementation shown in [Bootstrap modal show (long way)](/as-js/samples/bs_modal_load_long)

Used functions:

 * [bs.modal.load](/as-js/docs/bs_modal_load)

## Example

<div class="row mt-30">
    <div class="col-md-6">
        <button type="button"
            data-as='{
                "click": {
                    "bs.modal.load": {
                        "url": "./data/bs_modal.html"
                    }
                }
            }'
        >Load modal</button>
    </div>
</div>

## Source

``` html
<button type="button"
    data-as='{
        "click": {
            "bs.modal.load": {
                "url": "./data/bs_modal.html"
            }
        }
    }'
>Load modal</button>
```
