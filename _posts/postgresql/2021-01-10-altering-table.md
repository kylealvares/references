---
created: 2021-01-10 12:00:00 -500
layout: post
title: Altering a Table
permalink: postgresql/altering-table
categories: postgres
collections: 
    - postgres
---

The ```ALTER TABLE``` command is used to alter a table. 
Columns can be added or removed after a table is created.

## Adding a Column 
{: id="add-col"}

### Syntax

{% highlight sql %}
ALTER TABLE <table-name> ADD <column-name> <column-constraints>;
{% endhighlight %}

### Example

{% highlight sql %}
ALTER TABLE Companies 
ADD stock_symbol VARCHAR(5) UNIQUE, 
ADD stock_price REAL;
{% endhighlight %}

## Removing a Column 
{: id="remove-col"}

### Syntax

{% highlight sql %}
ALTER TABLE <table-name> DROP <column-name>;
{% endhighlight %}

### Example

{% highlight sql %}
ALTER TABLE Companies
DROP stock_symbol, 
DROP stock_price;
{% endhighlight %}