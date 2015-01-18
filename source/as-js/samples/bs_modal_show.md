---
layout: asjs
title: Bootstrap Modal Show - AS-JS Example
---

# bs.modal.show

This sample illustrates showing of a pre-loaded bootstrap modal. Note the modal is already in DOM when
``bs.modal.show`` is executed. It just triggers ``.modal('show')`` on it.

Used functions:

 * [bs.modal.show](/as-js/docs/bs_modal_show)

## Example

<div class="row mt-30">
    <div class="col-md-6">
        <button type="button"
            data-as='{
                "click": {
                    "bs.modal.show": {
                        "target": ".modal",
                        "removeOnClose": false
                    }
                }
            }'
        >Load modal</button>
    </div>
</div>

<div class="modal fade" id="bs_modal_id" role="dialog" aria-labeledby="xTitleID" aria-hidden="false">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-hidden="true">&times;</button>
                <h4 class="modal-title" id="xTitleID">Pre-loaded model</h4>
            </div>
            <div class="modal-body">
                <p>This modal was in the page when it was loaded.</p>
            </div>
            <div class="modal-footer">
                <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
            </div>
        </div>
    </div>
</div>

## Source

``` html
<button type="button"
    data-as='{
        "click": {
            "bs.modal.show": {
                "target": ".modal",
                "removeOnClose": false
            }
        }
    }'
>Load modal</button>

<div class="modal fade" id="bs_modal_id" role="dialog" aria-labeledby="xTitleID" aria-hidden="false">
...
</div
```
