## Issue Lifecycle

We use GitHub issues and ZenHub to manage our work.  Here's our major [board](https://github.com/SYNQfm/obaku#boards?repos=83064032,79477666,80748537,81571134,79564980,81447813,84829819,79788970,81179259) where you can see all of our issues across all of development repos.  Here's a helpful [guide](guidelines.md) for creating issues.

Issue Input -> Priority Analysis -> Schedule -> Work -> Test -> Deploy

### Walkthrough of a simple issue's life cycle

* Bruce discovers an issue in our /video/create call where it's returning extraneous metadata [information](https://github.com/SYNQfm/obaku/issues/601).
* He creates the issue in the `Obaku` repo, labels it a `bug` and puts it in `Weekly Milestone review`.  He puts `2` for the estimated effort
* On the subsequent monday, Bruce suggests to do it as its a quick fix and that it's pretty critical for the metadata integrity.  This is then moved into `Midgard week 12`, the current milestone release (Midgard) and the current week.  This is assigned to `batmany13` and placed in `In Progress`, `Planning/Design` was skipped as its pretty straight forward on how to fix it (change the migration to skip displaying that info if the state is not uploaded)
* Bruce has other issues he's working on, so the issue is placed under the one he's working on to show its priority.
* Bruce gets to the issue and fixes it, and submits a PR, change the issue's Pipeline to `Review/QA` board
* After the issue is reviewed, and accepted, it is merged into master and the issue is automatically moved to the `Closed` board

### Walkthrough of a more complicated issue's life cycle

* Bruce works with a customer to find that DVR for Live Streaming isn't working. He will
 * Create the issue on `streamer` [repo](https://github.com/SYNQfm/streamer/issues/75)
 * Set the appropriate tags to `help wanted` and `question`
 * Place it in the `Pending Schedule` Board
* In the Weekly Milestone Review, we look at `Weekly Milestone Review` and `Pending Schedule` board, and determine this needs to be fixed, so it gets moved to `Planning/Design`
* The issue is assigned to `batmany13`(Bruce) to fix
* Bruce has other issues he's working on, so he has to finish those before he can debug it, this takes 1 week before we gets to it.
* When he has time, he investigates the issue (by emailing Nimble support) and he finds that this is actually two issues, one is we have to setup a DVR for each output [stream](https://github.com/SYNQfm/streamer/issues/96) and we have to change the playback url to use the dvr m3u8 file instead of the abr [one](https://github.com/SYNQfm/streamer/issues/97)
* The original issue is closed, and the two new issues are created and placed into `Pending Schedule`
* On the subsequent Monday, the new issues are reviewed and the first one, issue 96 needs to be done first.  However, since the second issue is simple to do, they are done together.  We review the current `In Progress` board for Bruce and find that he has too many things to do, and placing these issues there would put him over 40 points.  Thus, these issues are moved to `Planning/Design`, as a "holding" areas of sorts, and will be moved over accordingly when he's finished with his other tasks.
* Finally, he finishes his other tasks, looks at his board filtered by "Assignee" (batmany13) and finds the two issues, and moves it into In-Progress
* After he finishes the first one 96, he issues a PR and moves the issue into the `Review/QA` pipeline.
* While issue 96 is being reviewed, he starts work on issue 97.  While working on it, he finds that there's a couple of sub tasks that needs to be done, so he adds the sub-task list to the issue and begins work on it.
* 96 is approved and merged into master, the issue is automatically moved to the `Closed` column
* 97 is completed, and is subsequently moved to `Review/QA`.  During the review, the PR specifically says that there is a deployment task that has to be done right after the deployment of code (change a setting in the database).  Thus, this issue is moved to `Post Deploy Work` to signify that it can't be closed until something is fixed on Deploy
* On the next Deploy day, the code is pushed out and the task was completed, now 97 is moved to the `Closed` board

## General Information

### Organization

* Epics - large scale work that encompasses multiple issues/tasks and could take several weeks.  Examples are like `Launch Live Streaming` or `Implement Dev/Test/Stage pipeline`
* Issues - individual bug/features or discussions needed to accomplish a task, should be tied with an Epic (unless there's general cleanup)
* Milestones - Major milestones are time based activities that include epics and issues.  This should typically be 1-2 months of time.  Subsequent "weekly" milestones are created to represent the on-going work to accomplish the major milestone.

### Board Overview

* Backlog - Issues filed, the general backlog
* Pending Schedule - This is what we need to look at every week
* Planning/Design - issues being designed or discussed.  This could be scheduled issues that require some planning or designing before starting work.  This could also be issues that are priority but require some debugging before determining course of action.
* In Progress - These are issues being actively worked on
* Review/QA - This typically means a PR is open for the release or it needs final testing
* Post Deploy Work - Issues that require some work after a deploy (or during)
* Closed - issue finished and ready to be deployed

### Milestones

* Weekly milestone review - Issues in this milestone will be reviewed every monday.
* "Current Milestone" (week xx) - This is the current weekly milestone, all issues here should've been reviewed
* "Milestone Name" (Next) - This is the milestone immediately proceeding the current milestone.  This should contain epics.  However, if there are a lot of issues, we should group them into a "theme" (or epic) and consolidate them.  Example is `Thule (Next)`

### What's the difference between milestones, boards and epics?

__Epics__ are _what_ we should be working on, and grouped by `subject`    
__Milestones__ is _when_ we work on issues, and grouped around `time`    
__Boards__ is _how_ we track what's being actively worked on now, how much work, spanned across all Repos    

Here's an [article](https://www.zenhub.com/blog/how-to-use-epics-and-milestones/) that talks about epics vs milestones

### Scheduling

* Issues should now be scheduled each monday into the current weekly milestone.  Also determine if we're on track for the current Milestone and what has to be adjusted
* The first monday of the month go through next milestone to see if there's clarification, epic creation, any themes that emerge
* The first Monday of each Quarter (Jan/April/July/Oct), review all issues in the backlog and determine if some should be closed or scheduled for next milestone review
* Developers are responsible for moving issues into the monthly review session, this means that you have to champion your features.
* Tech-lead is responsible for issues that non-developers wants championed.
* Issues can be inserted quite freely into the weekly review, if someone feels that it is important that we get to an issue.
* If an issue is broken down into smaller issues, those can be scheduled directly into the same week as parent issues was in and/or weekly/monthly review.