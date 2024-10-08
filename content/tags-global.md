---
title: '@global'
tag: global
tags: blockTags
layout: index.njk
description: Document a global object.
related:
    - /tags-inner
    - /tags-instance
    - /tags-memberof
    - /tags-static
---

## Overview

The `@global` tag specifies that a symbol should appear in the documentation as a _global_ symbol.
JSDoc ignores the symbol's actual scope within the source file. This tag is especially useful for
symbols that are defined locally, then assigned to a global symbol.


## Examples

Use the `@global`  tag to specify that a symbol should be documented as global.

::: example "Document an inner variable as a global"

```js
(function() {
    /** @global */
    var foo = 'hello foo';

    this.foo = foo;
}).apply(window);
```
:::
