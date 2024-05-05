# Assignment 1

## Motivation:

Software engineers make different types of design decisions, such as to create components or select technologies of a system. However, we know little about the impact of these decisions on the source code design, size and quality. This makes it hard to identify decisions from source code.

## Goal:

Explore differences and correlations in code quality and design changes for the different types of design decisions.

## Project

Map-Reduce

## Code

- [ ] [Github Link ](https://github.com/apache/hadoop) for finding commits

# Tasks:

## Week 1 : Explore software repository.

### 1. Determine commits that implement design issues:

1. Get the list of issue IDs where each issue ID is associated with one or more types of design decisions.
2. Determine the commits that implement the issues, and their parent commits.
3. _(Generally, the issue IDs are in the commit messages.)_ So, we need to loop on the commits to find the commit(s) that implement each issue using [PyDriller](https://pydriller.readthedocs.io/en/latest/index.html).
4. For issues IDs without a commit, we will exclude them for now.
5. After this, we will determine the parent commits.

### 2. Compile the software automatically through script:

1.  Create a script that can loop on the given commits, and compile the project, create a jar file or .class files.

    _Hint : This can be challenging, because sometimes the setting of the project change by time. Thus, try to rank the commits chronologically to know, which commits can be compiled in the same way, and
    adjust your scripts to be able to compile all commits._

### 3. Determine size and quality information of commit changes:

Using PyDriller, we will determine the following information for each commit:

1.  No. of added, modified and deleted files. (per commit)
2.  No. of added and deleted lines of code (per file)
3.  No. of added, deleted, and changed methods (per file)
4.  DMM metrics (per commit)
5.  Complexity (per file)

### 4. Generate Charts:

Given the collected size and quality information per commit, we will create charts such as boxplots that presents the

1. size information per decision type
2. quality information per decision type

_Hint: Remember that each commit is associated to an issue, which is associated to a decision type._

## Week 2 : Run clustering algorithms.

Details yet to be filled

## Week 3 : Analyze the results of clustering algorithms.

Details yet to be filled

### Git Details for Task 1

T1W1 : Task 1 Week 1 : Determine commits that implement design issues
compile_skript : Task 2 Week 1 : Compile the software automatically through script:
T3W1 : Task 3 Week 1 : Determine size and quality information of commit changes
T4W1 : Task 4 Week 1 : Generate Charts
Assignment_1.md -> information about Assignment 1
README.md -> information about the whole project from DS4SE Group 8
