---
layout: asjs
title: Bootstrap Modal Load (long way) - AS-JS Example
---

# Bootstrap modal show (long way)

This example demonstrates loading of remove bootstrap modal content and showing it once loaded. It makes a sequence of
[load](/as-js/doc/load), [html](/as-js/doc/html), and [bs.modal.show](/as-js/doc/bs_modal_show) functions.

Note there's a convenient shortcut implemented in [bs.modal.load](/as-js/doc/bs_modal_load) function, with example
in [Bootstrap modal show (short way)](/as-js/samples/bs_modal_load_short). This sample is just an illustration of
what function ``bs.modal.load`` does.

Used functions:

 * [load](/as-js/docs/load)
 * [html](/as-js/docs/html)
 * [bs.modal.show](/as-js/docs/bs_modal_show)

## Example

<div class="row mt-30">
    <div class="col-md-6">
        <button type="button"
            data-as='{
                "click": {
                    "load": {
                        "url": "./data/bs_modal.html",
                        "success": {
                            "html": {
                                "success": {
                                    "bs.modal.show": null
                                }
                            }
                        }
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
            "load": {
                "url": "./data/bs_modal.html",
                "success": {
                    "html": {
                        "success": {
                            "bs.modal.show": null
                        }
                    }
                }
            }
        }
    }'
>Load modal</button>
```
