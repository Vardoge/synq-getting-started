## Issue Lifecycle

We use GitHub issues and ZenHub to manage our work.  Here's a general flow

[Issue Input](guidelines.md) -> [Schedule](schedule.md) -> [Execute](../README.md#execute) -> [Deploy](../deploymd)


[Zenhub board](https://github.com/SYNQfm/obaku#boards?repos=83064032,79497430,79477666,80748537,74674362,81468857,90048135,81571134,79564980,81447813,84829819,79788970,81179259,88030190) 

## General Information


### Organization

* Epics - large scale work that encompasses multiple issues/tasks and could take several weeks.  Examples are like `Launch Live Streaming` or `Implement Dev/Test/Stage pipeline`
* Issues - individual bug/features or discussions needed to accomplish a task, should be tied with an Epic (unless there's general cleanup)
* Milestones - Major milestones are time based activities that include epics and issues.  This should typically be 1-2 months of time.

### Board Overview

* Backlog - Issues filed, the general backlog
* Pending Schedule - This is what we need to look at every week
* Selected for dev. - This is a holding area for issues that are queued up that should be done.  There shouldn't be more than 3-5 issues at a time.
* In Progress - These are issues being actively worked on.  There shouldn't be more than 2 issues at a time.
* Review/QA - This typically means a PR is open for the release or it needs final testing
* Post Deploy Work - Issues that require some work after a deploy (or during)
* Closed - issue finished and ready to be deployed

### Milestones

* "Milestone Name (Current)" - This is the current milestone, all epics (and maybe some issues) should live here.  The period is typically 1-2 months.  Example is `Midgard (Current)`
* "Milestone Name" (Next) - This is the milestone immediately proceeding the current milestone.  This should contain epics.  However, if there are a lot of issues, we should group them into a "theme" (or epic) and consolidate them.  Example is `Thule (Next)`

### What's the difference between milestones, boards and epics?

__Epics__ are _what_ we should be working on, and grouped by `subject`    
__Milestones__ is _when_ we work on issues, and grouped around `time`    
__Boards__ is _how_ we track what's being actively worked on now, how much work, spanned across all Repos    

Here's an [article](https://www.zenhub.com/blog/how-to-use-epics-and-milestones/) that talks about epics vs milestones

### Walkthrough of a simple issue's life cycle

* Bruce discovers an issue in our /video/create call where it's returning extraneous metadata [information](https://github.com/SYNQfm/obaku/issues/601).
* He creates the issue in the `Obaku` repo, labels it a `bug` and puts it in `Backlog` column.  He puts `2` for the estimated effort.  Bruce thinks it is a quick fix and that it's pretty critical for the metadata integrity, so he places it in `Pending Schedule`
* On the subsequent monday, the team reviews all the items in `Pending Schedule` and it's decided the issue should be fixed.  This is assigned to `batmany13` and placed in `In Progress` as Bruce has finished all his tasks.
* Bruce fixes the issue and submits a PR, and change the issue's Pipeline to `Review/QA` board
* After the issue is reviewed, and accepted, it is merged into master and the issue is automatically moved to the `Closed` board

### Walkthrough of a more complicated issue's life cycle

* Bruce works with a customer to find that DVR for Live Streaming isn't working. He will
  * Create the issue on `streamer` [repo](https://github.com/SYNQfm/streamer/issues/75)
  * Set the appropriate tags to `help wanted` and `question`
  * Place it in the `Pending Schedule` Board
* In the weekly review, we look at the `Pending Schedule` board, and determine this needs to be fixed, so it gets moved to `Selected for dev.`
* The issue is assigned to `batmany13`(Bruce) to fix
* Bruce has other issues he's working on, so he has to finish those before he can debug it, this takes 1 week before we gets to it.
* When he has time, he moves the issue from `Selected for dev.` to `In Progress`.
* He investigates the issue (by emailing Nimble support) and he finds that this is actually two issues, one is we have to setup a DVR for each output [stream](https://github.com/SYNQfm/streamer/issues/96) and we have to change the playback url to use the dvr m3u8 file instead of the abr [one](https://github.com/SYNQfm/streamer/issues/97)
* The original issue is closed, and the two new issues are created.
* The new issues will take a bit of time, and he has a smaller issue to work on, so he decides to place the two new issues in `Selected for dev.`
* When he finishes the small issue, Bruce filters his Zenhub board by "Assignee" (batmany13) and finds the two issues, and moves it into In-Progress
* After he finishes the first one 96, he issues a PR and moves the issue into the `Review/QA` pipeline.
* While issue 96 is being reviewed, he starts work on issue 97.  While working on it, he finds that there are a couple of sub tasks that needs to be done, so he adds the sub-task list to the issue and begins work on it.
* 96 is approved and merged into master, the issue is automatically moved to the `Closed` column
* 97 is completed, and is subsequently moved to `Review/QA`.  During the review, the PR specifically says that there is a deployment task that has to be done right after the deployment of code (change a setting in the database).  Thus, this issue is moved to `Post Deploy Work` to signify that it can't be closed until something is fixed on Deploy
* On the next Deploy day, the code is pushed out and the task was completed, now 97 is moved to the `Closed` board
