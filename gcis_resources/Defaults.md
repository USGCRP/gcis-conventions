# Default Conventions

## Identifier Conventions

### Introduction  
Assigning citable, unique and persistent identifiers to information held within the GCIS greatly increases the transparency and traceability of that
information as well as addressing a growing trend within the Federal research community: requiring researchers to formally cite the data and
document the processes that led to a given research result (Mayernik, et al., 2012).

### Title

The Resources title (or name, if no title field) is modified to be come the
identifier. Spaces are replaced with `-`. All letters are lowercased.

An older convention removed the words `in`, `and`, `&`, `on`, `the`, and `of` from titles. This is no longer preferred.

### UUID

A [UUID](../external_conventions/UUID.md) is generated for the resource and used as the identifier. Globally
unique.

### Number

The Resource type has an incrementing number as the identifier. Unique only for
a given resource.

## Ubiquitous Fields

### Introduction

Some fields have the same value regardless of which resource they appear on. They are described here for simplicity.

### Sort Key

Items with a sort key tend to be displayed in line with others of that resource type. For example, chapters of a report or authors on an article. 

Sort key is handled in ascending order. A resource with sort key 10 will apear about one with 20, which will both be above one with sort key 100.

Whenever external ordering is available, it should be respected. 

This value is not displayed to the end user.

