---
title: GitHub Flow
tags: [GitHub, Workflow]
style: fill
color: primary
description: GitHub Flow is a lightweight, branch-based workflow that supports teams & projects where deployments are made regularly. This guide explains how & why GitHub Flow works.
---

Source: [GitHub Guides](https://guides.github.com/introduction/flow/)

## Create a branch

When you're working on a project, you're going to have a bunch of different features or ideas in progress at any given time – some of which are ready to go, & others which aren't. Branching exists to help you manage this workflow.

When you create a branch in your project, you're creating an environment where you can try out new ideas. Changes you make on a branch don't affect the `master` branch, so you're free to experiment & commit changes, safe in the knowledge that your branch won't be merged until it's ready to be reviewed by someone you're collaborating with.

#### ProTip

Branching is a core concept in Git, & the entire GitHub flow is based upon it. There's only 1 rule: Anything in the `master` branch is always deployable.

Because of this, it's extremely important your new branch is created off of master when working on a feature or a fix. Your branch name should be descriptive (e.g., `refactor-authentication`, `user-content-cache-key`, `make-retina-avatars`), so others can see what's being worked on.

## Add commits

Once your branch has been created, it's time to start making changes. Whenever you add, edit, or delete a file, you're making a commit, & adding them to your branch. This process of adding commits keeps track of your progress as you work on a feature branch.

Commits also create a transparent history of your work others can follow to understand what you've done & why. Each commit has an associated commit message, which is a description explaining why a particular change was made. Furthermore, each commit is considered a separate unit of change. This lets you roll back changes if a bug is found, or if you decide to head in a different direction.

#### ProTip

Commit messages are important, especially since Git tracks your changes & then displays them as commits once they're pushed to the server. By writing clear commit messages, you can make it easier for other people to follow along & provide feedback.

## Open a Pull Request

Pull Requests initiate discussion about your commits. Because they're tightly integrated with the underlying Git repository, anyone can see exactly what changes would be merged if they accept your request.

You can open a Pull Request at any point during the development process: when you have little or no code but want to share some screenshots or general ideas, when you're stuck & need help or advice, or when you're ready for someone to review your work. By using GitHub's @mention system in your Pull Request message, you can ask for feedback from specific people or teams, whether they're down the hall or 10 time zones away.

#### ProTip

Pull Requests are useful for contributing to open source projects & for managing changes to shared repositories. If you're using a Fork & Pull Model, Pull Requests provide a way to notify project maintainers about the changes you'd like them to consider. If you're using a Shared Repository Model, Pull Requests help start code review & conversation about proposed changes before they're merged into the master branch.

## Discuss and review your code

Once a Pull Request has been opened, the person or team reviewing your changes may have questions or comments. Perhaps the coding style doesn't match project guidelines, the change is missing unit tests, or maybe everything looks great and props are in order. Pull Requests are designed to encourage and capture this type of conversation.

You can also continue to push to your branch in light of discussion & feedback about your commits. If someone comments you forgot to do something or if there's a bug in the code, you can fix it in your branch & push up the change. GitHub will show your new commits & any additional feedback you may receive in the unified Pull Request view.

#### ProTip

Pull Request comments are written in Markdown, so you can embed images & emoji, use pre-formatted text blocks, & other lightweight formatting.

## Deploy

With GitHub, you can deploy from a branch for final testing in production before merging to master.

Once your pull request has been reviewed & the branch passes your tests, you can deploy your changes to verify them in production. If your branch causes issues, you can roll it back by deploying the existing master into production.

## Merge

Now that your changes have been verified in production, it's time to merge your code into the master branch.

Once merged, Pull Requests preserve a record of the historical changes to your code. Because they're searchable, they let anyone go back in time to understand why & how a decision was made.

#### ProTip

By incorporating certain keywords into the text of your Pull Request, you can associate issues with code. When your Pull Request is merged, the related issues are also closed. For example, entering the phrase `Closes #32` would close issue number 32 in the repository.