---
created: 2021-01-02 12:00:00 -500
layout: post
title: Terminal Basics
permalink: postgresql/terminal-basics
categories: postgres
collections: 
    - postgres
---

PostgreSQL is available for download as ready-to-use packages or installers for various platforms, as well as a source code archive if you want to build it yourself. In addition PostgreSQL comes with a command line interface.
[Download PostgreSQL](https://www.postgresql.org/download/).

### Starting the terminal

When starting the psql terminal you will be asked to enter the connection information (as shown below). 
The default values are specified within the brackets.
If you want to use the default value just hit enter.

```https
Server [localhost]:
Database [postgres]:
Port [5432]:
Username [postgres]:
Password for user postgres: 
```

### Common psql commands

<table>
    <thead>
        <tr>
            <th>Command</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>\?</td>
            <td>Helps with psql commands</td>
        </tr>
        <tr>
            <td>\h</td>
            <td>Helps with sql commands</td>
        </tr>
        <tr>
            <td>\l</td>
            <td>Lists all of your databases</td>
        </tr>
        <tr>
            <td>\c [database]</td>
            <td>Connects to a database</td>
        </tr>
        <tr>
            <td>\d</td>
            <td>Describes the connected database</td>
        </tr>
        <tr>
            <td>\d [table]</td>
            <td>Describes a table</td>
        </tr>
        <tr>
            <td>\i [file]</td>
            <td>Executes commands from a file</td>
        </tr>
        <tr>
            <td>\q</td>
            <td>Quit</td>
        </tr>
    </tbody>
</table>
