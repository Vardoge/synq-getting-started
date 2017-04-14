# Guidelines for Issue Creation

Anyone in the organization can create issues (biz/sales/r&d/customer success), but they need to follow these simple guidelines below

## Tag it

__All issues on github _should_ have one of the following labels describing the type__

* Feature
* Task
* Improvement
* Bug
* Discussion

_Note: Issues can have other tags as well these are just the standard categories_

## Estimate how long it will take

Issues should have an "Estimate", which is the hours/points you think this will take.  This is just an estimate, and there might be an initial stab that gets updated to reflect the real work required.  This will be required to help balance the amount of work that can be done a week.

## Decide on the review priority

It is up to you to decide what the relative priority is of a specific issue.  Issues will typically fall into these categories

* Critical - production down issue or deploy issue that requires immediate attention, and may require patching
* Relevant/Required - This should be done in the current week or current milestone, is most likely highly reflective of what needs to be done to accomplish our epics.  This can include things like refactoring and improving tests, doesn't just have to be feature based
* Normal - This should be done over the course of one or two milestones
* Minor - this is small quick fixes like spelling mistakes, clean up bad referenced urls etc
* TODO - This would be a nice to have and should be eventually done, more like tracking high level features

Based on those priorities, you will place the issues in the follow states

* Critical - `In Progress` Pipeline, put into with current milestone, and escalate to team lead
* Relevant - Put into `Weekly Milestone Review`
* Normal - Put into `xxx (Next)` (the next milestone)
* Minor - Put into `Weekly Milestone Review` or `In Progress` (use your discretion)
* TODO - Leave in `Backlog` with no milestones attached

