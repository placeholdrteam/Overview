# Overview
Central repo for all planning and agiling the work flow. Do NOT fork this.

## How to edit this repo

As stated above, do **not** fork this repo as we do with the others. You may notice with this particular repo, we all have push access as collaborators. The idea is to create long-term branches, one for each collaborator. Those branches then are worked on individually, and merged into master when appropriate.

### Why we are using this approach

Since the purpose of this repo is an overview of the app in general, there is no need for a full-blown work flow to take place just to make planning edits. Add, or change what you need to on your own branch, then push that branch. Then merge it into master via a pull request on github. Preferrably, do not merge to your own master and push to the repo's master.

## What this repo is for

The purpose of this repo is for planning and vision ideas.

This is also where we keep the main project board.

* **If you have an idea**
  > Create an issue, with an enhancement tag, and perhaps an ideal release version to be included in. Also, assign it to the approriate person, project, and perhaps milestone *if you are using that process*
* **If you have a question**
  > Create an issue, with a question tag, and assign it to the individual you believe can answer it
* **If you are working on something**
  > Move it's issue card to the *In Progress* column manually, as there is not good automation to do this
* **If you have a mockup**
  > Add it either to the mockup folder (bad), or as a hosted link to the MockUps.md (better)
* **If you are moving a card to another board**
  > Tag it as assigned, and close the issue. This will move it to the done column, and will indicate it's functionality will be worked on in the appropriate repo. If you close an issue without tagging as assigned, it will be assumed to have been rejected, or taken care of within this repo already.

## Feature Process

* Pull from `central` remote
* Resolve any conflicts
  > In almost all cases, you should accept the `central` changes over your own in the case of conflicts
* Start a new feature with `git flow feature start <name>`
  > This will create and checkout that new branch for you.

  > This should be a *feature* branch, not *features*. Keep the changes isolated and as relevant as possible.
* Commit all your changes on this new branch until the feature is complete.
  > Commit often and commit well! Use clear commit messages. Clarity over brevity.
* Finish the feature with `git flow feature finish <name>`
  > This will do a `--no-ff` merge into your develop and place you on the develop branch
* Then push your new develop to your `origin` remote.
* **Immediately** go to your GitHub and submit a pull request to the central repo.
* Communicate with the GitHub Guru to review and accept your pull request
  > It is up to team to decide the appropriate changes to accept when merge conflicts occur, and the responsibility of the Guru to make the are resolved in a clean manner.
* Repeat (with a pull)
