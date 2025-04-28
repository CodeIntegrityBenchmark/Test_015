# Test_015
This project is part of a benchmark / test suite used to check the different git histories created through different development processes. The test suite is meant to be processed by SPHA-Code-Integrity.

## Textual Description
Expected Commits against integrity rules :
* All Commits expect the ones that are done via the PR, i.e. commits updating the expected Result file.

## Changes Made In This Repo

* Create a feature branch from main and make a commit on that branch.
* Create a second commit on the main branch.
* Create a sub-feature branch based on the feature branch and make a commit on the sub-feature branch
* Make a commit on the sub-feature that will conflict with feature.
* Make a commit on the feature branch that also conflicts with sub-feature
* Then make multiple commits on sub-feature branch and squash them and merge it with the sub-feature branch using a PR. Resolve conflicts.
* Create a third commit on the main branch that conflicts with the sub feature branch.
* Create multiple on the feature branch.
* Create a commit on main to update the Readme.
* Then merge the feature branch with the main branch without PR and using squash and merge.
* Create a commit on feature branch that updates the expected result JSON.
* Create a PR from feature to rebase with main for expected results.
