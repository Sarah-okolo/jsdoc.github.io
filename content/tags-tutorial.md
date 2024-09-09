---
title: '@tutorial'
tag: tutorial
tags: blockTags
layout: index.njk
description: Insert a link to an included tutorial file.
related:
    - /about-tutorials
    - /tags-inline-tutorial
    - /tags-see
---

## Syntax

    `@tutorial <tutorialID>`


## Overview

The `@tutorial` tag inserts a link to a tutorial file that is provided as part of the documentation.
See the [tutorials overview][tutorials] for instructions on creating tutorials.

You can use the `@tutorial` tag more than once in a single JSDoc comment.

[tutorials]: /about-tutorials


## Examples

In the following example, the documentation for `MyClass` will link to the tutorials that have the
identifiers `tutorial-1` and `tutorial-2`:

::: example "Using the @tutorial tag"

```js
/**
 * Description
 * @class
 * @tutorial tutorial-1
 * @tutorial tutorial-2
 */
function MyClass() {}
```
:::
