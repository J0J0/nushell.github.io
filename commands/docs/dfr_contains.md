---
title: dfr contains
categories: |
  dataframe
version: 0.90.0
dataframe: |
  Checks if a pattern is contained in a string.
usage: |
  Checks if a pattern is contained in a string.
feature: dataframe
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# <code>{{ $frontmatter.title }}</code> for dataframe

<div class='command-title'>{{ $frontmatter.dataframe }}</div>


::: warning
Dataframe commands were not shipped in the official binaries by default, you have to build it with `--features=dataframe` flag
:::
## Signature

```> dfr contains {flags} (pattern)```

## Parameters

 -  `pattern`: Regex pattern to be searched


## Input/output types:

| input | output |
| ----- | ------ |
| any   | any    |

## Examples

Returns boolean indicating if pattern was found
```nu
> [abc acb acb] | dfr into-df | dfr contains ab
╭───┬───────╮
│ # │   0   │
├───┼───────┤
│ 0 │ true  │
│ 1 │ false │
│ 2 │ false │
╰───┴───────╯

```
