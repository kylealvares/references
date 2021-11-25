---
created: 2021-10-10 18:38:00 -500
layout: post
title: Terminal Basics
permalink: postgresql/terminal-basics
categories: postgres
collections: 
    - postgres
toc: site.data.nav
---

PostgreSQL is available for download as ready-to-use packages or installers for various platforms, as well as a source code archive if you want to build it yourself. In addition PostgreSQL comes with a command line interface.
[Download PostgreSQL](https://www.postgresql.org/download/).

### Common psql commands

<table>
    <thead>
        <tr>
            <th>Terminology</th>
            <th>Example</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>\?</td>
            <td>Help with psql commands</td>
        </tr>
        <tr>
            <td>\h</td>
            <td>Help with sql commands</td>
        </tr>
        <tr>
            <td>\l</td>
            <td>Lists all of your databases</td>
        </tr>
        <tr>
            <td>\c [database]</td>
            <td>Connect to a database</td>
        </tr>
        <tr>
            <td>\d [database / table]</td>
            <td>Describes a database / table</td>
        </tr>
        <tr>
            <td>\q</td>
            <td>Quit</td>
        </tr>
    </tbody>
</table>
