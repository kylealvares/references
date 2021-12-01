---
created: 2021-01-05 12:00:00 -500
layout: post
title: Creating a Table
permalink: postgresql/create-table
categories: postgres
collections: 
    - postgres
---

The ```CREATE TABLE``` command is used to create a table in SQL.

Tables are created within databases.
To create a table you will need to list out the column names, and specify their data types.

<h3 id="common-data-types">Common data types</h3>

<table>
    <thead>
        <tr>
            <th>Data type</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>int / integer</td>
            <td>whole numbers (-2147483648 to +2147483647)</td>
        </tr>
        <tr>
            <td>real / float</td>
            <td>decimal values (6 decimal digits precision)</td>
        </tr>
        <tr>
            <td>char(n)</td>
            <td>text of fixed length, blank padded</td>
        </tr>
        <tr>
            <td>varchar(n)</td>
            <td>text of varying length up to 'n' characters</td>
        </tr>
        <tr>
            <td>text</td>
            <td>text of unlimited length</td>
        </tr>
        <tr>
            <td>date</td>
            <td>'yyyy-mm-dd' (ex. '2021-11-25')</td>
        </tr>
        <tr>
            <td>time</td>
            <td>'hh:mm:ss' (ex. '15:30:02.5' - 2.5s after 3:30p.m.)</td>
        </tr>
    </tbody>
</table>

Note that values can be set to ```NULL```. 
To ensure a value is not null, use the ```NOT NULL``` constraint.

### Syntax

{% highlight sql %}
CREATE TABLE <table-name> (
    <column-name> <data-type> NOT NULL,
    <column-name> <data-type>,
    <column-name> <data-type>,
    ...
);
{% endhighlight %}

### Example

{% highlight sql %}
CREATE TABLE Companies (
    name TEXT,
    type TEXT,
    founded INT,
    hq TEXT
);
{% endhighlight %}

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
            <td>\d [table]</td>
            <td>Describes a table</td>
        </tr>
    </tbody>
</table>