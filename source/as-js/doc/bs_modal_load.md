---
layout: asjs
title: Bootstrap modal load - AS-JS
---

bs.modal.load
=============

Loads remote bootstrap modal content, adds it do DOM, and shows it. When modal is closed it removes it from DOM.

It's a convenient shortcut method that calls those three functions as shown in
[Bootstrap modal load (long way)](/as-js/samples/bs_modal_load_long).

Options
-------

 * ``url`` - required, string, url to load content from


Example HTML
------------

``` html
<button type="button"
    data-as='{
        "click": {
            "bs.modal.load": {
                "url": "bs_modal.html"
            }
        }
    }'
>Load modal</button>
```

Example javascript
------------------

``` js
AS.execute($('#dom', {
    load: {
        url: "http://example.com/modal.html"
    }
});
```
