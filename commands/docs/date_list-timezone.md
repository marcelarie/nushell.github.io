---
title: date list-timezone
categories: |
  date
version: 0.85.0
date: |
  List supported time zones.
usage: |
  List supported time zones.
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# <code>{{ $frontmatter.title }}</code> for date

<div class='command-title'>{{ $frontmatter.date }}</div>

## Signature

```> date list-timezone ```


## Input/output types:

| input   | output |
| ------- | ------ |
| nothing | table  |

## Examples

Show timezone(s) that contains 'Shanghai'
```shell
> date list-timezone | where timezone =~ Shanghai
╭───┬───────────────╮
│ # │   timezone    │
├───┼───────────────┤
│ 0 │ Asia/Shanghai │
╰───┴───────────────╯

```
