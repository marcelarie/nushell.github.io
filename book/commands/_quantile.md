---
title: quantile
version: 0.64.0
usage: |
  Aggregates the columns to the selected quantile
---

<script>
  import { usePageFrontmatter } from '@vuepress/client';
  export default { computed: { frontmatter() { return usePageFrontmatter().value; } } }
</script>

# <code>{{ frontmatter.title }}</code>

<div style='white-space: pre-wrap;'>{{ frontmatter.usage }}</div>

## Signature

```> quantile (quantile)```

## Parameters

 -  `quantile`: quantile value for quantile operation

## Examples

quantile value from columns in a dataframe
```shell
> [[a b]; [6 2] [1 4] [4 1]] | to-df | quantile 0.5
```