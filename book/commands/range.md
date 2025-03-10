---
title: range
layout: command
version: 0.60.0
usage: |
  Return only the selected rows.
---

# `{{ $frontmatter.title }}`

<div style='white-space: pre-wrap;'>{{ $frontmatter.usage }}</div>

## Signature

```> range (rows)```

## Parameters

 -  `rows`: range of rows to return: Eg) 4..7 (=> from 4 to 7)

## Examples

Get the last 2 items
```shell
> [0,1,2,3,4,5] | range 4..5
```

Get the last 2 items
```shell
> [0,1,2,3,4,5] | range (-2)..
```

Get the next to last 2 items
```shell
> [0,1,2,3,4,5] | range (-3)..-2
```
