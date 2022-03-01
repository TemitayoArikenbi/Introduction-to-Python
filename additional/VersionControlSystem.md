# Version Control Systems

## What is version control?

Version control, also known as source control, is the practice of tracking and managing changes to software code. Version control systems are software tools that help software teams manage changes to source code over time. As development environments have accelerated, version control systems help software teams work faster and smarter. They are especially useful for DevOps teams since they help them to reduce development time and increase successful deployments.

Version control software keeps track of every modification to the code in a special kind of database. If a mistake is made, developers can turn back the clock and compare earlier versions of the code to help fix the mistake while minimizing disruption to all team members.

Version Control Systems (VCS) have seen great improvements over the past few decades and some are better than others. VCS are sometimes known as SCM (Source Code Management) tools or RCS (Revision Control System). One of the most popular VCS tools in use today is called Git. Git is a Distributed VCS, a category known as DVCS. Like many of the most popular VCS systems available today, Git is free and open source. Regardless of what they are called, or which system is used, the primary benefits you should expect from version control are as follows.

## How version control works

Version control systems enable code tracking, which creates a record of code changes, and deltas, which highlight the differences between file versions. When teams can see their full history, they are also able to merge, which enables teams to combine new changes with existing code, and revert, which helps them go back to previous versions. 

When teams use version control, they can better organize and coordinate changes to their codebase made by everyone on their team. Any changes are visible to the entire team, who can then use their version control system as a way to track and share their code changes with other team members. 

Most teams today use distributed version control, which keeps a database of changes on a single server and distributes local copies to each developer. Whenever a developer needs to see the latest changes to the codebase, she can access them on the server and sync them to her local version control. If she makes changes to the codebase on her local machine, she can also push those changes to the server, making them accessible to everyone else on her team. 

## Centralized Version Control Systems vs. Distributed Version Control Systems

The main difference between centralized and distributed version control is that, in centralized version control, the versions are saved in the remote repository, while in distributed version control, versions can be saved in the remote repository as well as in local repositories of the local machines.

## Version Control System Examples

### Centralized Version Control Systems
- Concurrent Version System (CVS)
- Apache Subversion

### Distributed Version Control Systems
- Git
- Mercurial
- Perforce Helix Core

## Git
Git is a free and open source distributed version control system. It is fast, efficient, and cross-platform. Git supports non-linear development with commands for creating branches and rewriting history. 

### Github
GitHub, a repository hosting service that implements Git VCS. Git keeps a historical record of all changes made to the codebase, while GitHub provides an easy way to sync and share those changes. 

Unlike some VCSs that only track deltas between files, Git takes a full snapshot of all files at each commit, whether or not they have changed. When using Git, every clone of a code repository is a complete backup; it contains all the necessary information to see how the repository has changed over time from the moment it was created. As a result, Git is a resilient and robust version control system. 
