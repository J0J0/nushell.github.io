---
title: dfr dtypes
categories: |
  dataframe
version: 0.90.0
dataframe: |
  Show dataframe data types.
usage: |
  Show dataframe data types.
feature: dataframe
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# <code>{{ $frontmatter.title }}</code> for dataframe

<div class='command-title'>{{ $frontmatter.dataframe }}</div>


::: warning
Dataframe commands were not shipped in the official binaries by default, you have to build it with `--features=dataframe` flag
:::
## Signature

```> dfr dtypes {flags} ```


## Input/output types:

| input | output |
| ----- | ------ |
| any   | any    |

## Examples

Dataframe dtypes
```nu
> [[a b]; [1 2] [3 4]] | dfr into-df | dfr dtypes
╭───┬────────┬───────╮
│ # │ column │ dtype │
├───┼────────┼───────┤
│ 0 │ a      │ i64   │
│ 1 │ b      │ i64   │
╰───┴────────┴───────╯

```
