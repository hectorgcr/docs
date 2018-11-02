---
title: GET
linkTitle: GET
description: GET
menu:
  v1.0:
    parent: api-redis
    weight: 2070
---

## Synopsis
<b>`GET key`</b><br>
This command fetches the value that is associated with the given `key`.

<li>If the `key` does not exist, null is returned.</li>
<li>If the `key` is associated with a non-string value, an error is raised.</li>

## Return Value
Returns string value of the given `key`.

## Examples
```{.sh .copy .separator-dollar}
$ GET yugakey
```
```sh
(null)
```
```{.sh .copy .separator-dollar}
$ SET yugakey "YugaByte"
```
```sh
"OK"
```
```{.sh .copy .separator-dollar}
$ GET yugakey
"YugaByte"
```

## See Also
[`append`](../append/), [`getrange`](../getrange/), [`getset`](../getset/), [`incr`](../incr/), [`incrby`](../incrby/), [`mget`](../mget/), [`mset`](../mset/), [`set`](../set/), [`setrange`](../setrange/), [`strlen`](../strlen/)