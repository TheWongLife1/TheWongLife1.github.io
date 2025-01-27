---
title: What's version control?
tags: [Version Control]
style: fill
color: secondary
comments: true
description: Benefits of version control & version control systems.
---

Source: [atlassian](https://www.atlassian.com/git/tutorials/what-is-version-control)

![](https://wac-cdn.atlassian.com/dam/jcr:34e935dd-3108-40ef-bb3d-9ed01d977d6d/hero.svg?cdnVersion=la)

## Benefits of version control

Version control systems are a category of software tools that help a software team manage changes to source code over time. Version control software keeps track of every modification to the code in a special kind of database. If a mistake is made, developers can turn back the clock & compare earlier versions of the code to help fix the mistake while minimizing disruption to all team members.

For almost all software projects, the source code is like the crown jewels - a precious asset whose value must be protected. For most software teams, the source code is a repository of the invaluable knowledge & understanding about the problem domain which the developers have collected & refined through careful effort. Version control protects source code from both catastrophe & the casual degradation of human error & unintended consequences.

Software developers working in teams are continually writing new source code & changing existing source code. The code for a project, app or software component is typically organized in a folder structure or "file tree". 1 developer on the team may be working on a new feature while another developer fixes an unrelated bug by changing code, each developer may make their changes in several parts of the file tree.

Version control helps teams solve these kinds of problems, tracking every individual change by each contributor & helping prevent concurrent work from conflicting. Changes made in 1 part of the software can be incompatible with those made by another developer working at the same time. This problem should be discovered & solved in an orderly manner without blocking the work of the rest of the team. Further, in all software development, any change can introduce new bugs on its own & new software can't be trusted until it's tested. So testing & development proceed together until a new version is ready.

Good version control software supports a developer's preferred workflow without imposing 1 particular way of working. Ideally it also works on any platform, rather than dictate what operating system or tool chain developers must use. Great version control systems facilitate a smooth & continuous flow of changes to the code rather than the frustrating & clumsy mechanism of file locking - giving the green light to 1 developer at the expense of blocking the progress of others.

Software teams which don't use any form of version control often run into problems like not knowing which changes which have been made are available to users or the creation of incompatible changes between 2 unrelated pieces of work which must then be painstakingly untangled & reworked. If you're a developer who has never used version control you may have added versions to your files, perhaps with suffixes like "final" or "latest" & then had to later deal with a new final version. Perhaps you've commented out code blocks because you want to disable certain functionality without deleting the code, fearing there may be a use for it later. Version control is a way out of these problems.

Version control software is an essential part of the every-day of the modern software team's professional practices. Individual software developers who are accustomed to working with a capable version control system in their teams typically recognize the incredible value version control also gives them even on small solo projects. Once accustomed to the powerful benefits of version control systems, many developers wouldn't consider working without it even for non-software projects.

## Benefits of version control systems

Developing software without using version control is risky, like not having backups. Version control can also enable developers to move faster & it allows software teams to preserve efficiency and agility as the team scales to include more developers.

Version Control Systems (VCS) have seen great improvements over the past few decades and some are better than others. VCS are sometimes known as SCM (Source Code Management) tools or RCS (Revision Control System). 1 of the most popular VCS tools in use today is called Git. Git is a Distributed VCS, a category known as DVCS, more on that later. Like many of the most popular VCS systems available today, Git is free & open source. Regardless of what they're called, or which system is used, the primary benefits you should expect from version control are as follows.

1. A complete long-term change history of every file. This means every change made by many individuals over the years. Changes include the creation and deletion of files as well as edits to their contents. Different VCS tools differ on how well they handle renaming & moving of files. This history should also include the author, date & written notes on the purpose of each change. Having the complete history enables going back to previous versions to help in root cause analysis for bugs & it's crucial when needing to fix problems in older versions of software. If the software is being actively worked on, almost everything can be considered an "older version" of the software.

1. Branching & merging. Having team members work concurrently is a no-brainer, but even individuals working on their own can benefit from the ability to work on independent streams of changes. Creating a "branch" in VCS tools keeps multiple streams of work independent from each other while also providing the facility to merge that work back together, enabling developers to verify that the changes on each branch don't conflict. Many software teams adopt a practice of branching for each feature or perhaps branching for each release, or both. There are many different workflows which teams can choose from when they decide how to make use of branching & merging facilities in VCS.

1. Traceability. Being able to trace each change made to the software & connect it to project management & bug tracking software like Jira, & being able to annotate each change with a message describing the purpose and intent of the change can help not only with root cause analysis & other forensics. Having the annotated history of the code at your fingertips when you're reading the code, trying to understand what it's doing & why it's so designed can enable developers to make correct & harmonious changes which are in accord with the intended long-term design of the system. This can be especially important for working effectively with legacy code & is crucial in enabling developers to estimate future work with any accuracy.

While it's possible to develop software without using any version control, doing so subjects the project to a huge risk which no professional team would be advised to accept. So the question isn't whether to use version control but which version control system to use.

There are many choices, but here we're going to focus on just 1, Git.