---
created: 2014-1-1 18:38:00 -500
layout: post
title: Introduction
permalink: sqa/introduction
collections: sqa
toc: site.data.sqa
---

**Quality Assurance (QA)** is the study of methods and disciplines for achieving quality results.

Quality is not a single idea, as it has many aspects. 
*Popularly*, quality is often associated with **perception**. 
*Professionally*, there is an **ethical imperative** to quality, but even further than that it is a
professional responsibility, a **moral** and **legal** requirement. 


From a professional standpoint quality should be measurable, this includes:
* Conformance to requirements - including timeliness, cost.
* Fitness for use - does it actually do the job?
* Freedom from errors and failures - is it reliable and robust?
* Customer satisfaction - are users happy with it? 

**Software quality** is the degree to which a system, component, or process meets:
* the **specified requirements**
* the customer's or **user's needs** or expectations

Software quality is discussed in terms of several different dimensions, which are referred to as quality parameters.
The two groups of parameters are **technical** and **user** quality parameters.


## Technical Quality Parameters

Technical quality parameters are open to **objective** measures and **technical solutions**. 

<table>
    <thead>
        <th>Parameter</th>
        <th>Description</th>
        <th>Measured By</th>
    </thead>
    <tbody>
        <tr>
            <td>Correctness</td>
            <td>Lack of bugs and defects</td>
            <td>Defect rate (# of bugs / line of code)</td>
        </tr>
        <tr>
            <td>Reliability</td>
            <td>Does not fail or crash often</td>
            <td>Failure rate (# of failures / hour)</td>
        </tr>
        <tr>
            <td>Capability</td>
            <td>Does all that is required</td>
            <td>Requirements coverage (% if requirements implemented)</td>
        </tr>
        <tr>
            <td>Maintainability</td>
            <td>Ability to adapt to meet new requirements</td>
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
        </tr>
    </tbody>
</table>


## User Quality Parameters

User quality parameters often require **subjective analysis** and **nontechnical solutions**.

<table>
    <thead>
        <th>Parameter</th>
        <th>Description</th>
        <th>Measured By User Satisfaction</th>
    </thead>
    <tbody>
        <tr>
            <td>Usability</td>
            <td>Sufficiently convenient for intended users</td>
            <td>% of users happy with interface and ease of use</td>
        </tr>
        <tr>
            <td>Installability</td>
            <td>Convenient and fast to install</td>
            <td># of install problems reported per installation</td>
        </tr>
        <tr>
            <td>Documentation</td>
            <td>Well documented</td>
            <td>% of users happy with documentation</td>
        </tr>
        <tr>
            <td>Availability</td>
            <td>Easy to access and available when needed</td>
            <td>% of users reporting access problems</td>
        </tr>
    </tbody>
</table>