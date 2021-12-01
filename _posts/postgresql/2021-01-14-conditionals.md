---
created: 2021-01-14 12:00:00 -500
layout: post
title: Conditionals
permalink: postgresql/conditionals
categories: postgres
collections: 
    - postgres
---

The ```WHERE``` clause is used to specify conditions of the queried result.
It can be used with ```AND```, ```OR``` and ```NOT``` for more complex conditionals.

The ```AND``` and ```OR``` operators are used for multiple conditions.
* ```AND``` evaluates to ```true``` when both sides of the condition are met.
* ```OR``` evaluates to ```true``` when ad least of the sides of the condition is met.

The ```NOT``` operator is used to specify when a condition is not true. 

### Syntax

{% highlight sql %}
SELECT <columns> FROM <table-name> WHERE <condition>
{% endhighlight %}

### Example #1

{% highlight sql %}
SELECT name, founded, hq FROM Companies WHERE hq='United States'; 
{% endhighlight %}

<table>
    <caption>Result from Example #1</caption>
    <thead>
        <tr>
            <th>Name</th>
            <th>Founded</th>
            <th>HQ</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Walmart</td>
            <td>1962</td>
            <td>United States</td>
        </tr>
        <tr>
            <td>Disney</td>
            <td>1923</td>
            <td>United States</td>
        </tr>
        <tr>
            <td>PayPal</td>
            <td>1998</td>
            <td>United States</td>
        </tr>
    </tbody>
</table>

### Example #2

{% highlight sql %}
SELECT name, founded, hq FROM Companies 
WHERE founded=1998 OR hq='Canada'; 
{% endhighlight %}

<table>
    <caption>Result from Example #2</caption>
    <thead>
        <tr>
            <th>Name</th>
            <th>Founded</th>
            <th>HQ</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>PayPal</td>
            <td>1998</td>
            <td>United States</td>
        </tr>
        <tr>
            <td>Blackberry</td>
            <td>1984</td>
            <td>Canada</td>
        </tr>
    </tbody>
</table>

### Example #3

{% highlight sql %}
SELECT name, founded, hq FROM Companies 
WHERE hq='United States' AND 
(founded='1923' OR founded='1998'); 
{% endhighlight %}

<table>
    <caption>Result from Example #3</caption>
    <thead>
        <tr>
            <th>Name</th>
            <th>Founded</th>
            <th>HQ</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Disney</td>
            <td>1923</td>
            <td>United States</td>
        </tr>
        <tr>
            <td>PayPal</td>
            <td>1998</td>
            <td>United States</td>
        </tr>
    </tbody>
</table>

### Example #4

{% highlight sql %}
SELECT name, founded, hq FROM Companies 
WHERE hq='United States'
ORDER BY founded; 
{% endhighlight %}

<table>
    <caption>Result from Example #4</caption>
    <thead>
        <tr>
            <th>Name</th>
            <th>Founded</th>
            <th>HQ</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Disney</td>
            <td>1923</td>
            <td>United States</td>
        </tr>
        <tr>
            <td>Walmart</td>
            <td>1962</td>
            <td>United States</td>
        </tr>
        <tr>
            <td>PayPal</td>
            <td>1998</td>
            <td>United States</td>
        </tr>
    </tbody>
</table>

### Example #5

{% highlight sql %}
SELECT name, founded, hq FROM Companies 
WHERE NOT hq='United States'; 
{% endhighlight %}

<table>
    <caption>Result from Example #5</caption>
    <thead>
        <tr>
            <th>Name</th>
            <th>Founded</th>
            <th>HQ</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Blackberry</td>
            <td>1984</td>
            <td>Canada</td>
        </tr>
    </tbody>
</table>