---
created: 2021-01-15 12:00:00 -500
layout: post
title: Comparisons
permalink: postgresql/comparisons
categories: postgres
collections: 
    - postgres
---

Comparison operators are operators that evaluate to ```true``` or ```false```.

<table>
    <caption>List of comparison operators</caption>
    <thead>
        <tr>
            <th>Operator</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>=</td>
            <td>equals</td>
        </tr>
        <tr>
            <td><</td>
            <td>less than</td>
        </tr>
        <tr>
            <td>></td>
            <td>greater than</td>
        </tr>
        <tr>
            <td><=</td>
            <td>less than or equal to</td>
        </tr>
        <tr>
            <td>>=</td>
            <td>greater than or equal to</td>
        </tr>
        <tr>
            <td><></td>
            <td>does not equal</td>
        </tr>
    </tbody>
</table>

### Syntax

{% highlight sql %}
SELECT <columns> FROM <table-name> WHERE <condition>; 
{% endhighlight %}

### Example 
{% highlight sql %}
SELECT name, founded FROM Companies WHERE founded < 1980; 
{% endhighlight %}

<table>
    <caption>Result from Example #1</caption>
    <thead>
        <tr>
            <th>Name</th>
            <th>Founded</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Walmart</td>
            <td>1962</td>
        </tr>
        <tr>
            <td>Disney</td>
            <td>1923</td>
        </tr>
    </tbody>
</table>