---
created: 2021-01-05 12:00:00 -500
layout: post
title: Inserting Values
permalink: postgresql/inserting-values
categories: postgres
collections: 
    - postgres
---

The ```INSERT INTO``` command is used to insert a single or multiple rows of values into a table.

### Syntax

```https
INSERT INTO <table-name> (<list-of-attributes>) 
VALUES (<list-of-values>);
```

### Example

```https
INSERT INTO Companies (name, type, founded, hq) 
VALUES ('Walmart', 'Retail', 1962, 'United States'),
('Disney', 'Entertainment', 1923, 'United States'),
('Paypal', 'Finance', 1998, 'United States'),
('Blackberry', 'Technology', 1984, 'Canada');
```

[Mockaroo](https://mockaroo.com/){: target="blank"} allows you to generate up to 1,000 rows of realistic test data in CSV, JSON, **SQL**, and Excel formats.

### Useful psql commands

<table>
    <thead>
        <tr>
            <th>Command</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>\i [file]</td>
            <td>Executes commands from a file</td>
        </tr>
    </tbody>
</table>