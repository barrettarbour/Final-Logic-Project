<!-- [![Work in Repl.it](https://classroom.github.com/assets/work-in-replit-14baed9a392b3a25080506f3b7b6d57f295ec2978f6f33ec97e36a161684cbe9.svg)](https://classroom.github.com/online_ide?assignment_repo_id=315694&assignment_repo_type=GroupAssignmentRepo)

# CISC/CMPE 204 Modelling Project

Welcome to the major project for CISC/CMPE 204 (Fall 2020)!

Change this README.md file to summarize your project (few sentences at most), and provide pointers to the general structure of the repository. How you organize and build things (which files, how you structure things, etc) is entirely up to you! The only things you must keep in place are what is already listed in the **Structure** section below. -->

# Group 12 CISC204 Modelling Project - Settlers of Catan

## Summary

Our project uses the concepts of logic in computing science to model a problem faced in a hypothetical game of Settlers of Catan, with the rules of the game slightly altered to be appropriate for a logical model. Given a certain board state in Settlers of Catan, where we know which tiles of a certain resource type (wood, sheep, wheat, brick) are connected to which other tiles, we would like to determine k the lowest number of steps required to find a winning path.

## Rules of the Model

In Settlers of Catan, players take turns traversing through the game board to gather resources. The full ruleset of the game is quite extensive, so we have altered the rules to suit our model. Our model considers the following:

-   The "board" is a tree (graph)? of connected nodes
-   There are four types of nodes, each representing a different resource: brick, sheep, wheat, and wood
-   The "board state" is a configuration that tells us how many nodes are in the board, what the type of each node is, and which nodes are connected to which other nodes.
-   A "branch" of the board is a path through the tree that starts at the root node and ends at a terminal node?
-   A "winning path" is a branch? path? that contains at least one node for each required resource

## Structure

-   `documents`: Contains folders for both of your draft and final submissions. README.md files are included in both.
-   `run.py`: General wrapper script that you can choose to use or not. Only requirement is that you implement the one function inside of there for the auto-checks.
-   `test.py`: Run this file to confirm that your submission has everything required. This essentially just means it will check for the right files and sufficient theory size.

## Documentation

This README.md provides a brief summary of the project and overview of the rules of the model. Extensive documention of the modelling process can be found in `documents/final/modelling_report.pptx`
