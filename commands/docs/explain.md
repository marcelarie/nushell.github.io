---
title: explain
categories: |
  debug
version: 0.85.0
debug: |
  Explain closure contents.
usage: |
  Explain closure contents.
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# <code>{{ $frontmatter.title }}</code> for debug

<div class='command-title'>{{ $frontmatter.debug }}</div>

## Signature

```> explain (closure)```

## Parameters

 -  `closure`: the closure to run


## Input/output types:

| input   | output |
| ------- | ------ |
| any     | any    |
| nothing | any    |
## Examples

Explain a command within a closure
```shell
> explain {|| ls | sort-by name type -i | get name } | table -e

```
