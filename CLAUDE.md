# Project

This repository contains rules and guidelines for helping people build software
for learning purposes. A description will be given about what the topic and goal
of the project is. The output should be a project split into milestones in a
separate directory.

## General principles

The goal is to break down complex topics into parts that are easier to
understand and implement.

It is desirable to start with imperfect solutions, which are then incrementally
improved in the following milestones.

## Rules

Setup should include:

1. Environment overview
2. Tools to install
3. How to run them

Each milestone must include:

1. Starting problem, if it is an incremental improvement of the previous
   milestone, highlight what the issue is with the previous solution
2. What is the desired result of the milestone
3. Components to be implemented
4. Communication between components

Always include diagrams where applicable.

Milestones don't need to make components perfect from the start. It is
acceptable and also desired that milestones build on top of previous ones with
incremental improvements.

Last milestone should always be about using production ready tools.

Verification should always consist of executable commands.

Example:

```bash

pytest

curl localhost:8000/health

make test
```

At the end, a document describing real world usage should be created.

## Workflow

1. People describe what they want to build and which concepts they want to learn
2. Claude generates guidelines and validation commands for the project split
   into parts that can be ran and validated
3. Claude generates a document presenting real world examples of desired project
   (if applicable), or how it is used
4. People can validate the output using provided commands

## Desired results

If the wants to work in `../project-dir`, Claude should create `../project-dir`.
In project dir, there should be two documents:

1. setup.md
2. miltestones/ (which each milestone in a separate file)
3. real-world-examples.md
