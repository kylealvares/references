---
created: 2021-01-22 12:00:00 -500
layout: post
title: Arithmetic Operators
permalink: postgresql/arithmetic-operators
collections: postgres
---

Basic arithmetic operations can be done using SQL command line interface.  

### Syntax

```https
SELECT <expression>;
```

<table>
    <!-- <caption>Common aggregate functions</caption> -->
    <thead>
        <tr>
            <th>Operator Name</th>
            <th>Operator</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Addition</td>
            <td>+</td>
            <td>Adds values together.</td>
        </tr>
        <tr>
            <td>Subtraction</td>
            <td>-</td>
            <td>Subtracts values.</td>
        </tr>
        <tr>
            <td>Multiplication</td>
            <td>*</td>
            <td>Performs multiplication operation.</td>
        </tr>
        <tr>
            <td>Divison</td>
            <td>/</td>
            <td>Adds values together.</td>
        </tr>
        <tr>
            <td>Modulus</td>
            <td>%</td>
            <td>Returns the remainder of statement.</td>
        </tr>
        <tr>
            <td>Exponent</td>
            <td>^</td>
            <td>Returns the remainder of statement.</td>
        </tr>
        <tr>
            <td>Factorial</td>
            <td>!</td>
            <td>Returns the remainder of statement.</td>
        </tr>
    </tbody>
</table>

### Example #1

```https
SELECT 10 * 2;
```

<table>
    <caption>Returns the value of 10 * 2</caption>
    <thead>
        <tr>
            <th>?column?</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>20</td>
        </tr>
    </tbody>
</table>

### Example #2

```https
SELECT 5!;
```

<table>
    <caption>Returns the value of 5 factorial</caption>
    <thead>
        <tr>
            <th>?column?</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>120</td>
        </tr>
    </tbody>
</table>