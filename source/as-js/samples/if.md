---
layout: asjs
title: If - AS-JS Example
---

# If

## Example

<div class="row">
    <div class="col-md-6">
        <button type="button"
            data-as='{
                "click": {
                    "if": {
                        "arg": {
                            "true": null
                        },
                        "then": {
                            "html": {
                                "result": "Then part",
                                "target": "#target"
                            }
                        }
                    }
                }
            }'
        >Then part</button>
        <button type="button"
            data-as='{
                "click": {
                    "if": {
                        "arg": {
                            "false": null
                        },
                        "else": {
                            "html": {
                                "result": "Else part",
                                "target": "#target"
                            }
                        }
                    }
                }
            }'
        >Else part</button>
    </div>

    <div id="target" class="col-md-6">
        ...
    </div>
</div>

<div class="mt-30"></div>

## Source

``` html
<button type="button"
    data-as='{
        "click": {
            "if": {
                "arg": {
                    "true": null
                },
                "then": {
                    "html": {
                        "result": "Then part",
                        "target": "#target"
                    }
                }
            }
        }
    }'
>Then part</button>
<button type="button"
    data-as='{
        "click": {
            "if": {
                "arg": {
                    "false": null
                },
                "else": {
                    "html": {
                        "result": "Else part",
                        "target": "#target"
                    }
                }
            }
        }
    }'
>Else part</button>
```
