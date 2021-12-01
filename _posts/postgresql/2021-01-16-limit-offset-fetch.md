---
created: 2021-01-15 12:00:00 -500
layout: post
title: Limit, Offset, Fetch
permalink: postgresql/limit-offset-fetch
categories: postgres
collections: 
    - postgres
---

### Limit

The ```LIMIT``` clause limits the amount of retrieved rows based on the specified limit.

#### Syntax

{% highlight sql %}
SELECT <columns> FROM <table-name> LIMIT <limit>; 
{% endhighlight %}

#### Example

{% highlight sql %}
SELECT * FROM Companies LIMIT 3; 
{% endhighlight %}

<table>
    <caption>First 3 rows of the Companies</caption>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Founded</th>
            <th>HQ</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Walmart</td>
            <td>Retail</td>
            <td>1962</td>
            <td>United States</td>
        </tr>
        <tr>
            <td>Disney</td>
            <td>Entertainment</td>
            <td>1923</td>
            <td>United States</td>
        </tr>
        <tr>
            <td>PayPal</td>
            <td>Finance</td>
            <td>1998</td>
            <td>United States</td>
        </tr>
    </tbody>
</table>

### Offset

The ```OFFSET``` clause offsets the first set of rows given by an ```ORDER BY``` clause.

#### Syntax

{% highlight sql %}
SELECT <columns> FROM <table-name>
ORDER BY <attribute-name>
OFFSET <offset>; 
{% endhighlight %}

#### Example

{% highlight sql %}
SELECT * FROM Companies
ORDER BY name
OFFSET 2
LIMIT 1; 
{% endhighlight %}

<table>
    <caption>1 row from Companies ordered by name offset by 2</caption>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Founded</th>
            <th>HQ</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>PayPal</td>
            <td>Finance</td>
            <td>1998</td>
            <td>United States</td>
        </tr>
    </tbody>
</table>

### Fetch

The ```FETCH``` clause is used with ```ORDER BY``` and ```OFFSET``` to retrieve rows.

#### Syntax

{% highlight sql %}
SELECT <columns> FROM <table-name>
ORDER BY <attribute-name>
OFFSET <offset>
FETCH <fetch-details>; 
{% endhighlight %}

#### Example

{% highlight sql %}
SELECT * FROM Companies
ORDER BY name
OFFSET 2
FETCH FIRST 2 ROW ONLY; 
{% endhighlight %}

<table>
    <caption>2 rows fetched from Companies, ordered by name, offset by 2</caption>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Founded</th>
            <th>HQ</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>PayPal</td>
            <td>Finance</td>
            <td>1998</td>
            <td>United States</td>
        </tr>
        <tr>
            <td>Walmart</td>
            <td>Retail</td>
            <td>1962</td>
            <td>United States</td>
        </tr>
    </tbody>
</table>