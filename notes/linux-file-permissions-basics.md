# Linux File Permissions Basics

## What are file permissions?
Linux file permissions define who can read, write, or execute a file.

## Permission groups
There are three main groups:
- owner
- group
- others

## Permission types
- r = read
- w = write
- x = execute

## Example
`rwxr-xr--`

This means:
- owner: read, write, execute
- group: read, execute
- others: read only

## Useful commands
- `ls -l`
- `chmod`
- `chown`

## Why this matters in cybersecurity
Permissions help control access and reduce unnecessary exposure of files and systems.
