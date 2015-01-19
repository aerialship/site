---
layout: asjs
title: AS-JS Documentation
---

AS-JS Documentation
===================

AS-JS automatically binds registered functions as DOM event listeners according to declarative specification in
``data-as`` attribute. Content of ``data-as`` attribute must be a valid json object. Field names represent event
names, while field value is an object which fields function names, while values are arguments that function arguments.

```
data-as = {
    "event-name-one": {
        "function-one": argument-A,
        "function-two": argument-B
    },
    "event-name-two": {
        "function-three": argument-C,
        "function-one": argument-D
    }
}
```

With a declaration above, triggering an ``event-name-one`` event on such DOM will execute sequentially ``function-one``
with ``argument-A`` and then ``function-two`` with ``argument-B``.

Each function receives only one argument variable. When called in it's argument value defined in ``data-as`` are
injected some standard values:

 * ``dom`` - DOM object event was triggered on
 * ``$dom`` - jQuery object wrapped around ``dom``
 * ``domEvent`` - browser event object that triggered the execution
 * ``result`` - result of previous function of the same event

For all browser DOM events, on elements with ``data-as`` attribute that functions are bind to, by default propagation
is stopped and default action prevented.

By adding ``data-as-stop-propagation="false"`` attribute you can allow propagation of the event.
By adding ``data-as-prevent-default="false"`` you can allow default event action.


Functions
---------

 * [bs.modal.load](/as-js/doc/bs_modal_load)
 * [html](/as-js/doc/html)
 * [load](/as-js/doc/load)
