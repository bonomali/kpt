---
title: "Count"
linkTitle: "count"
weight: 4
type: docs
description: >
   Print resource counts for a package
---

{{< asciinema key="cfg-count" rows="10" preload="1" >}}

Count quickly summarizes the number of resources in a package.

### Examples

```sh
# print Resource counts from a directory
kpt cfg count my-dir/
```

```sh
# print Resource counts from a cluster
kubectl get all -o yaml | kpt cfg count
```

### Synopsis

    kpt cfg count [DIR]

    DIR:
      Path to a package directory.  Defaults to stdin if unspecified.
