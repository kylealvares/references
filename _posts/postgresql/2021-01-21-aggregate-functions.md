---
created: 2021-01-21 12:00:00 -500
layout: post
title: Aggregate Functions
permalink: postgresql/aggregate-functions
collections: postgres
---

Aggregate functions are single values computed from several rows of data.
These functions include `MAX`, `MIN`, `AVG`, `ROUND` and `SUM`.

Check out the [PostgreSQL's full list of aggregate functions](https://www.postgresql.org/docs/14/functions-aggregate.html).

### Common aggregate functions

<table>
    <!-- <caption>Common aggregate functions</caption> -->
    <thead>
        <tr>
            <th>Function</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Max</td>
            <td>Computes the max of non-null input values.</td>
        </tr>
        <tr>
            <td>Min</td>
            <td>Computes the min of non-null input values.</td>
        </tr>
        <tr>
            <td>Avg</td>
            <td>Computes the average (arithmetic mean) of all the non-null input values.</td>
        </tr>
        <tr>
            <td>Round</td>
            <td>Rounds of all the non-null input values. Round can also specify the amount of decimal places with a second argument.</td>
        </tr>
        <tr>
            <td>Sum</td>
            <td>Computes the sum of the non-null input values.</td>
        </tr>
    </tbody>
</table>

### Syntax

```https
SELECT <aggregate-function>(<column>) FROM <table>;
```

### Example #1
```https
SELECT MAX(founded) FROM Companies;
```

<table>
    <caption>The max value in the <code>founded</code> column.</caption>
    <thead>
        <tr>
            <th>Max</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1998</td>
        </tr>
    </tbody>
</table>

> Note: In some cases, an aggregate function can be used within another. <br>
> For example: `ROUND(AVG(price), 2)`, rounds the average value of `price` up to two decimal places.

### Example #2
```https
SELECT hq, MIN(founded) FROM Companies 
GROUP BY hq;
```

<table>
    <caption>The <code>hq</code> and <code>min</code> of each hq group </caption>
    <thead>
        <tr>
            <th>HQ</th>
            <th>Min</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>United States</td>
            <td>1923</td>
        </tr>
        <tr>
            <td>Canada</td>
            <td>1984</td>
        </tr>
    </tbody>
</table>

