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

{% highlight sql %}
INSERT INTO <table-name> (<list-of-attributes>) 
VALUES (<list-of-values>);
{% endhighlight %}

### Example

{% highlight sql %}
INSERT INTO Companies (name, type, founded, hq) 
VALUES ('Walmart', 'Retail', 1962, 'United Stated'),
VALUES ('Disney', 'Entertainment', 1923, 'United Stated'),
VALUES ('Paypal', 'Finance', 1998, 'United Stated'),
VALUES ('Blackberry', 'Technology', 1984, 'Canada');
{% endhighlight %}


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