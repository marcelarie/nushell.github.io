---
title: math arctanh
categories: |
  math
version: 0.85.0
math: |
  Returns the inverse of the hyperbolic tangent function.
usage: |
  Returns the inverse of the hyperbolic tangent function.
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# <code>{{ $frontmatter.title }}</code> for math

<div class='command-title'>{{ $frontmatter.math }}</div>

## Signature

```> math arctanh ```


## Input/output types:

| input        | output       |
| ------------ | ------------ |
| list\<number\> | list\<number\> |
| number       | number       |
## Examples

Get the arctanh of 1
```shell
> 1 | math arctanh
inf
```


**Tips:** Command `math arctanh` was not included in the official binaries by default, you have to build it with `--features=extra` flag