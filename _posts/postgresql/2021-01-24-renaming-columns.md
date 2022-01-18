---
created: 2021-01-22 12:00:00 -500
layout: post
title: Renaming Columns
permalink: postgresql/renaming-columns
collections: postgres
---

The `AS` clause allows for columns to be aliased or renamed in a query.

### Syntax

```https
SELECT <column> AS <alias> FROM <table>;
```

### Example

```https
SELECT name AS Company FROM Companies;
```

<table>
    <caption>The <code>name</code> column renamed as <code>Company</code></caption>
    <thead>
        <tr>
            <th>Company</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Walmart</td>
        </tr>
        <tr>
            <td>Disney</td>
        </tr>
        <tr>
            <td>PayPal</td>
        </tr>
        <tr>
            <td>Blackberry</td>
        </tr>
    </tbody>
</table>