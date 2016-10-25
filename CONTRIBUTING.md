# How to contribute

We're striving to keep master's history with minimal merge bubbles. To achieve this, we're asking pull requests to be submitted rebased 
on top of master.

To keep your local repository in a "rebased" state, simple run:

```bash
$ git config --global
```

```bash
$ branch.autosetuprebase always
```
_changes the default for all future Branches_

```bash
git config --global
```
```bash
$ branch.master.rebase true 
```
_changes the setting for branch master_

Note: you may still have to run manual "rebase" commands on your branches, to rebase on top of master as you pull changes from upstream.


## Finding things to work on

The first place to start is always looking over the current github issues for the project you are interested in contributing to.Issues 
marked with _help wanted_ are usually pretty self contained and a good place to get started. Chamaconekt also uses these same github 
issues to keep track of what we are working on.If you see any issues that are assigned to a particular person that means someone is 
currently working on that issue.

Of course feel free to make your own issues if you think something needs to be added or fixed.


## Basic quality checks

Please ensure that all tests pass before submitting changes.

Try to separate logically distinct changes into separate commits and thematically distinct commits into separate pull requests.

## Submitting changes

Please sign the [Contributor License Aggreement]() .

All content, comments, and pull requests must follow the [Chamaconekt Community Guidelines]()

Submit a pull request rebased on top of master
- Include a descriptive commit message
- Changes contributed via pull requests should focus on a sigle issues at a time.

At this point you're waiting on us.We like to at least comment on pull requests within one week (and typically, three business days).
We may suggest some changes or improvements or alternatives.

