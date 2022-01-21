---
created: 2021-9-23 18:38:00 -500
layout: post
title: Stack vs Heap Memory
permalink: algorithms/stack-vs-heap
collections: algorithms
toc: site.data.algorithms
---

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


<table>
    <thead>
        <th>Parameter</th>
        <th>Description</th>
        <th>Measured By</th>
        <th>Measured By</th>
    </thead>
    <tbody>
        <tr>
            <td>Correctness</td>
            <td>Lack of bugs and defects</td>
            <td>Defect rate (# of bugs / line of code)</td>
            <td>Defect rate (# of bugs / line of code)</td>
        </tr>
        <tr>
            <td>Reliability</td>
            <td>Does not fail or crash often</td>
            <td>Failure rate (# of failures / hour)</td>
            <td>Failure rate (# of failures / hour)</td>
        </tr>
        <tr>
            <td>Capability</td>
            <td>Does all that is required</td>
            <td>Requirements coverage (% if requirements implemented)</td>
            <td>Requirements coverage (% if requirements implemented)</td>
        </tr>
        <tr>
            <td>Maintainability</td>
            <td>Ability to adapt to meet new requirements</td>
            <td>Change logs (time & effort required to add feature)<br> 
                Impact Analysis (# of lines affected with new requirement)
            </td>
            <td>Change logs (time & effort required to add feature)<br> 
                Impact Analysis (# of lines affected with new requirement)
            </td>
            <td>Change logs (time & effort required to add feature)<br> 
                Impact Analysis (# of lines affected with new requirement)
            </td>
            <td>Change logs (time & effort required to add feature)<br> 
                Impact Analysis (# of lines affected with new requirement)
            </td>
            <td>Change logs (time & effort required to add feature)<br> 
                Impact Analysis (# of lines affected with new requirement)
            </td>
            <td>Change logs (time & effort required to add feature)<br> 
                Impact Analysis (# of lines affected with new requirement)
            </td>
            <td>Change logs (time & effort required to add feature)<br> 
                Impact Analysis (# of lines affected with new requirement)
            </td>
            <td>Change logs (time & effort required to add feature)<br> 
                Impact Analysis (# of lines affected with new requirement)
            </td>
        </tr>
        <tr>
            <td>Performance</td>
            <td>Speed and memory efficient</td>
            <td>Speed (CPU time)<br>
                Memory (Mb of memory)
            </td>
            <td>Speed (CPU time)<br>
                Memory (Mb of memory)
            </td>
        </tr>
    </tbody>
</table>