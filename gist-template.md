# Regular Expressions (Regex) Tutorial
## What is a Regex?
"Regular Expressions," or "Regex," is a sequence of special characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be:
-used to find certain patterns of characters within a string
-used to find and replace a characted or sequence of characters within a string 
-used to validate input

For example, the following regular expression can be used to verify that user input is a valid email address:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

Each component of this regex has a unique responsibility to make sure that a user enters an email address that begins with an unspecified number of characters preceding the `@` symbol, followed by a domain.
## Summary 

In this tutorial, I will explain what different component parts do for a specific regex. 

For the purposes of this demonstration, I will break down "Matching a Hex Value" regex to obtain a better understanding of regular expressions and their components.

Matching a Hex Value: `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

## Table of Conetents 
- [Anchors](#anchors)
-
