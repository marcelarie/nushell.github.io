---
title: from nuon
categories: |
  formats
version: 0.85.0
formats: |
  Convert from nuon to structured data.
usage: |
  Convert from nuon to structured data.
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# <code>{{ $frontmatter.title }}</code> for formats

<div class='command-title'>{{ $frontmatter.formats }}</div>

## Signature

```> from nuon ```


## Input/output types:

| input  | output |
| ------ | ------ |
| string | any    |

## Examples

Converts nuon formatted string to table
```shell
> '{ a:1 }' | from nuon
╭───┬───╮
│ a │ 1 │
╰───┴───╯
```

Converts nuon formatted string to table
```shell
> '{ a:1, b: [1, 2] }' | from nuon
╭───┬───────────╮
│ a │ 1         │
│   │ ╭───┬───╮ │
│ b │ │ 0 │ 1 │ │
│   │ │ 1 │ 2 │ │
│   │ ╰───┴───╯ │
╰───┴───────────╯
```
