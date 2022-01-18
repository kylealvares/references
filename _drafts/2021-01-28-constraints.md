---
created: 2021-01-27 12:00:00 -500
layout: post
title: Constraints
permalink: postgresql/constraints
collections: postgres
---

# 25, 26, 27 - Incomplete
- link to other constraint topics

Constriants are restrictions put on a table.

## Finding a constraint's name

1. Use the `\d <table>` command to view the table's details.
2. The **Indexes** portion should contain details regarding the constraints. <br>
Find the constraint name.

## Adding a constraint

### Syntax

```https
ALTER <table> TABLE ADD PRIMARY KEY (<column(s)>);
```

## Removing a constraint

### Syntax

```https
ALTER <table> DROP CONSTRAINT <primary-key-name>;
```

## Check constraint
