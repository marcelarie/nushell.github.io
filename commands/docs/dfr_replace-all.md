---
title: dfr replace-all
categories: |
  dataframe
version: 0.77.0
dataframe: |
  Replace all (sub)strings by a regex pattern.
usage: |
  Replace all (sub)strings by a regex pattern.
---

# <code>{{ $frontmatter.title }}</code> for dataframe

<div class='command-title'>{{ $frontmatter.dataframe }}</div>

## Signature

```> dfr replace-all ```

## Examples

Replaces string
```shell
> [abac abac abac] | dfr into-df | dfr replace-all -p a -r A
╭───┬──────╮
│ # │  0   │
├───┼──────┤
│ 0 │ AbAc │
│ 1 │ AbAc │
│ 2 │ AbAc │
╰───┴──────╯

```