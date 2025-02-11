---
title: str distance
categories: |
  strings
version: 0.85.0
strings: |
  Compare two strings and return the edit distance/Levenshtein distance.
usage: |
  Compare two strings and return the edit distance/Levenshtein distance.
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# <code>{{ $frontmatter.title }}</code> for strings

<div class='command-title'>{{ $frontmatter.strings }}</div>

## Signature

```> str distance (compare-string) ...rest```

## Parameters

 -  `compare-string`: the first string to compare
 -  `...rest`: For a data structure input, check strings at the given cell paths, and replace with result


## Input/output types:

| input  | output |
| ------ | ------ |
| record | record |
| string | int    |
| table  | table  |
## Examples

get the edit distance between two strings
```shell
> 'nushell' | str distance 'nutshell'
1
```

Compute edit distance between strings in table and another string, using cell paths
```shell
> [{a: 'nutshell' b: 'numetal'}] | str distance 'nushell' 'a' 'b'
╭───┬───┬───╮
│ # │ a │ b │
├───┼───┼───┤
│ 0 │ 1 │ 4 │
╰───┴───┴───╯

```

Compute edit distance between strings in record and another string, using cell paths
```shell
> {a: 'nutshell' b: 'numetal'} | str distance 'nushell' a b
╭───┬───╮
│ a │ 1 │
│ b │ 4 │
╰───┴───╯
```
