---
created: 2021-9-23 18:38:00 -500
layout: post
title: Asymptotic Notation
permalink: algorithms/asymptotic-notation
collections: algorithms
toc: site.data.algorithms
---

Asymptotic notation describes the **running time** of an algorithm through functions that
the set of natural numbers ```ℕ = {0, 1, 2,...}``` as their domain. 
This notation is convenient for determining worst-case run time scenarios ```T(n)```.
However in some cases asyptotic notation can extend the domain to the set of real numbers or restrict it to 
a subset of the natural numbers.

The amount of time it takes for code to run varies not only between devices, but also between runs.
This is due to the fact that time is affected by factors such as hardware, programming language, number of applications open, and so on.
As a result, rather than measuring the time it takes a program to run, it is preferable to count the number of operations and see how it changes as input size increases.

![big oh, theta and omega graphs](../assets/img/analysis-design-algorithms/asymptotic-notation-light.svg)
{: class="light-version" }

![big oh, theta and omega graphs](../assets/img/analysis-design-algorithms/asymptotic-notation-dark.svg)
{: class="dark-version" }

<div class="caption">Big theta, oh and omega graphs</div>

## Big Oh (O) Notation

*O*(*n*) is an **upper bound** asymptotic notation.

*O*(*g*(*n*)) = { *f*(*n*): there exists postive constants *c* and *n*<sub>0</sub> such that **0 ≤ *f*(*n*) ≤ *cg*(*n*)** for all *n* ≥ *n*<sub>0</sub> }

Example: 2*n*<sup>2</sup> = *O*(*n*<sup>3</sup>), where *c* = 1 and *n*<sub>0</sub> = 2

Examples of *O*(*n*<sup>2</sup>): *n*<sup>2</sup>, *n*<sup>2</sup> + *10n*, *n*  

## Big Omega (Ω) Notation

*Ω*(*n*) is a **lower bound** asymptotic notation.

*Ω*(*g*(*n*)) = { *f*(*n*): there exists postive constants *c* and *n*<sub>0</sub> such that **0 ≤ *cg*(*n*) ≤ *f*(*n*)** for all *n* ≥ *n*<sub>0</sub> }

Example: √*n* = *Ω*(lg *n*), where *c* = 1 and *n*<sub>0</sub> = 16

Examples of *Ω*(*n*<sup>2</sup>): *n*<sup>2</sup>, *n*<sup>2</sup> + *10n*, 2<sup>*n*</sup> 

## Big Theta (Θ) Notation

*Θ*(*n*) is an **exact value** or **useful range** that narrows the performance of an algorithm.

*Θ*(*g*(*n*)) = { *f*(*n*): there exists postive constants *c*<sub>1</sub>, *c*<sub>2</sub>, and *n*<sub>0</sub> such that **0 ≤ *c*<sub>1</sub>*g*(*n*) ≤ *f*(*n*) ≤ *c*<sub>2</sub>*g*(*n*)** for all *n* ≥ *n*<sub>0</sub> }

Example: *n*<sup>2</sup> / 2 - 2*n* = *Θ*(*n*<sup>2</sup>), where  *c*<sub>1</sub> = 1/4, *c*<sub>2</sub> = 1/2, and *n*<sub>0</sub> = 8.

**Theorem:** *f*(*n*) = *Θ*(*g*(*n*)) if and only if *f* = *O*(*g*(*n*)) and *f* = *Ω*(*g*(*n*)).

## Functions

Check out this [Big Oh Cheatsheet](https://www.bigocheatsheet.com/){: target="_blank" } for an overview of big-oh notation for various data structures and functions.

<table>
    <caption>Functions from least to greatest time complexity</caption>
    <thead>  
        <tr>
            <th>Function</th>
            <th>Notation</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Constant</td>
            <td>1</td>
        </tr>
        <tr>
            <td>Logarithmic</td>
            <td>log<em>n</em></td>
        </tr>
        <tr>
            <td>Square Root</td>
            <td>√<em>n</em></td>
        </tr>
        <tr>
            <td>Linear</td>
            <td><em>n</em></td>
        </tr>
        <tr>
            <td>Loglinear</td>
            <td><em>n</em>log<em>n</em></td>
        </tr>
        <tr>
            <td>Quadratic</td>
            <td><em>n</em><sup>2</sup></td>
        </tr>
        <tr>
            <td>Cubic</td>
            <td><em>n</em><sup>3</sup></td>
        </tr>
        <tr>
            <td>Polynomial</td>
            <td><em>n</em><sup><em>k</em></sup></td>
        </tr>
        <tr>
            <td>Exponential</td>
            <td>2<sup><em>n</em></sup></td>
        </tr>
        <tr>
            <td>Factorial</td>
            <td><em>n</em>!</td>
        </tr>
    </tbody>
</table>

<!-- **Rule book for O notation**
1. Consider the worst case
2. Remove constants
3. Different terms for inputs
4. Drop Non Dominants    -->
