---
title: arg-min
version: 0.69.1
dataframe: |
  Return index for min value in series
usage: |
  Return index for min value in series
---

# <code>{{ $frontmatter.title }}</code> for dataframe

<div style='white-space: pre-wrap;margin-top: 10px'>{{ $frontmatter.dataframe }}</div>

## Signature

```> arg-min ```

## Examples

Returns index for min value
```shell
> [1 3 2] | into df | arg-min
```