# Query Lint VS Code
Language-Server implementation for VS Code providing linting and query validation for JavaScript ASTs

## Purpose and Context
Much of my role involves writing scripts that query ASTs of user code runs.
We use [ESPrima](https://esprima.org/) to parse user code into ASTs, and [ESQuery](https://github.com/estools/esquery)
to query AST nodes. This is how I verify if a user has completed a puzzle, and if not, determines which feedback message
the user is shown.

This process involes a lot of switching between browser and VS Code, and with limited monitor space, this can be
mildly disruptive to the workflow.

This project allows one to write a block of code in between comments, and then write the queries below.
Hovering the mouse cursor over the query will display the node returned by the query.

## Project Status

This is still a work in progress, and is not yet ready to replace the [AST parsing site](https://bcorman.github.io/esquery-training/)
that I mainly use for content creation.

As this is not currently deployed to the VS Code extension marketplace, testing of the repo must be done in VS Code debug mode.
