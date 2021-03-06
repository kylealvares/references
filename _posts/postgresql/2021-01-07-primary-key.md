---
created: 2021-01-07 12:00:00 -500
layout: post
title: Primary Key
permalink: postgresql/primary-key
collections: postgres
---

A key is **an attribute or set of attributes that are used to uniquely identify a tuple in a relation**.
Keys can also be used to establish relations between other relations and columns. 
The values of a key are called key values.

A ```PRIMARY KEY``` is **the attribute that identifies a each row in a table**.
If multiple attributes form a primary key this is known as a **composite key**. 
There can only be one primary key per table. Each primary key value must be unique and cannot be ```NULL```.

### Syntax

```https
CREATE TABLE <table-name> (
    <column-name> <column-type> PRIMARY KEY,
    <column-name> <column-type>,
    ...
);
```

### Example

```https
CREATE TABLE Companies (
    name TEXT PRIMARY KEY,
    type TEXT,
    founded INT,
    hq TEXT,
);
```

<h2 id="composite-key">Composite Keys</h2>

A composite key is **the set of attributes that identifies a each row in a table**.

```https
CREATE TABLE Companies (
    name TEXT,
    type TEXT,
    founded INT,
    hq TEXT,
    PRIMARY KEY(Name, Founded)
);
```
