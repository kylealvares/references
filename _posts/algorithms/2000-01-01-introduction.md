---
created: 2021-9-23 18:38:00 -500
layout: post
title: Introduction
permalink: algorithms/introduction
collections: algorithms
toc: site.data.algorithms
---

Algorithms are steps for solving a problem. 
There are several algorithms like cooking food or sorting numbers.

## Basic Terminology

<dl>
<dt>Alogrithm</dt>
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