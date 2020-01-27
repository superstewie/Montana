# Branching Guidelines
<!-- Put some introductory text here -->
Montana uses a branching strategy very closely based on [gitflow](https://nvie.com/posts/a-successful-git-branching-model/).
This document lays out in full detail the specific branching strategy and related terminology that we use.

<!-- Should I build graphics to describe the three categories? -->
<!-- Then, describe the three categories of branches -->
We divide branches into three broad categories:
- _Permanent_ branches which once created always exist and never change
  - Are used to create indestructable snapshots of the state of the project at a moment in time
- _Long Lived_ branches which always exist, but can be committed to more than once
  - Are used to create running records of the projects state over time
- _Short Lived_ branches which are created and destroyed at will
  - Are used to modify the state of the project

<!-- Finally, classify the actual branch types into the categories -->
There are six concrete branch types:
- The _master_ branch is a long lived branch used to record the distributable state of the project
- The _development_ branch is a long lived branch used to record all work done on the project
- _release_ branches are short lived branches used to prepare a development commit for merging into the _master_ branch
- _feature_ branches are short lived branches used to do work on the project
- _hotfix_ branches are short lived branches used to fix problems in the master branch
- _build_ branches are permanent branches used to record build artifacts from the master branch
<!-- build branches could have many uses. Two possibilities are building nuget packages and creating
     entry points for Long-Term Support versions. 

#### Branching Rules

<!-- Here I want to describe the rules of working with branches -->
<!-- I want to make sure to layout the commands to be used in foreseeable situations -->

![Graph describing the branching flow](BranchDirection.png)

*Fig. 1 describes where each type of branch comes from, as well as where each type of branch can be merged to.*

