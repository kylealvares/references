---
created: 2021-9-23 18:38:00 -500
layout: post
title: Introduction
permalink: algorithms/introduction
collections: algorithms
toc: site.data.algorithms
---

To write good code, developers must take advantage of data structures and algorithms.
A good developer must understand the trade off between **readability**, **memory**, and **speed**.

## Basic Terminology

<dl>
<dt>Data Structure</dt>
<dd>A <strong>collection of values</strong>, that can have <strong>relationships</strong> and <strong>functions</strong>.
<li>Each data structure is different and <strong>specialized</strong> for different purposes.</li>
<li>Common data structures include <i>arrays</i>, <i>lists</i>, <i>stacks</i>, <i>queues</i>, <i>maps</i>, <i>trees</i>, etc.</li></dd>
<dt>Algorithm</dt>
<dd>An algorithm is any well-defined computational procedure that
    <li> Takes some value, or set of values, as <strong>input</strong>.</li>
    <li>Produces some value, or set of values, as <strong>output</strong>.</li>
    <li>An algorithm should be <strong>correct</strong> and <strong>efficient</strong>.</li>
</dd>
<dt>Design</dt>
<dd>Method for developing an algorithm.</dd>
<dt>Analysis</dt>
<dd>Abstract mathematical comparison of algorithms.</dd>
</dl>

## Analyzing Algorithms

There are several items to consider when analyzing algorithms including: 

* Time Complexity (CPU)
* Spatial Complexity (Disk & Memory)
* Correctness
* Termination

## Pseudocode

An algorithm is a step by step procedure to solving a task,
whereas pseudocode is a method for writing an algorithm.

### Fibonacci Psuedocode:
```https
Fib(n):
1   if n == 0 or n == 1
2       return 1
3   else 
4       return Fib(n - 1) + Fib(n - 2)
```

<!-- ## Case Study: Insertion Sort
```https
incomplete
``` -->