---
menu:
  main:
    parent: "Core Language"
title: "Databases"
weight: 6
---

# Databases

databases contain records

## Syntax

```eve
// search action
search @database

search (@database1, ..., @databaseN)

// Commit action
commit @database

commit (@database1, ..., @databaseN)

// Bind action
bind @database

bind (@database1, ..., @databaseN)
```

## Description

`<action> @database` performs the given action, one of `search`, `bind`, or `commit`, on the provided database.

`<action> (@database1, ..., @databaseN)` performs the given action, on the union of the provided databases. For instance `` 

If no database is provided with an action, then that action is performed on the default `@session` database.

## Special Databases

- `@event`

- `@browser` 

- `@session`

## Examples



## See Also

[search](../search) | [bind](../bind) | [commit](../commit)