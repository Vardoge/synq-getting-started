## Scheduling

Each week there will be `30` hours of scheduled work per developer.  This is done on purpose so that there is extra wiggle room to allow for meetings, code reviews, minor ad-hoc fixes and critical production issues.  There are two main ways issues are assigned to a developer, through `weekly` meetings and `ad-hoc` scheduling.

### Weekly Meetings

* There is a Developers Meeting every Monday.  This is where we will review issues in the `Pending Schedule` board to be moved to the `Selected for dev.` board.  We will also review the `In Progress` and `Selected for dev.` boards to see the progress we are making.
* There should never be over `45` hours of work between `Selected for dev.` and `In Progress`.  If an issue has to be scheduled in, then previously `Selected for dev.` issues need to be removed
* Developers are responsible for championing their issues that they feel are strong.
* Tech-lead is responsible for issues that non-developers wants championed.
* Issues can be inserted quite freely into `Pending Schedule`, if someone feels that it is important that we get to an issue.
* If an issue is broken down into smaller issues, those can be scheduled directly into the same week as parent issue

### Ad-hoc Scheduling

* Issues can and will come up during the week.  We want to give room for this, and that is what ad-hoc scheduling is for.
* Ad-hoc issues should either be `critical issues` found during a production impacting event or `minor fixes` which will not exceed `5` hours of work per issue.  `DevOps`, `Outage` and build pipeline issues should be referred to the person in the DevOps rotation (listed below)
* There should only be 2-3 ad-hoc issues scheduled a week.  They should not domniate your week's work, and if you are busy with a key task, do not schedule these in, place it in `Pending Schedule` instead.
* Your `In Progress` and `Selected for dev.` should not exceed `45` hours.
* _Use your own discretion!_
* If a `critical issue` will cause your weekly scheduled issues to be delayed, let the `team lead` know

### Monthly and Quarterly Reviews

* The first monday of the month go through next milestone to see if there's clarification, epic creation, any themes that emerge
* The first Monday of each Quarter (Jan/April/July/Oct), review all issues in the backlog and determine if some should be closed or scheduled for next milestone review

### DevOps Rotational Role

Each week, the developer on `DevOps` Rotation is responsible for

* Tagging and writing the release notes on Monday and deploying the code on Tuesday
* Deal with any deploy issues during or after the release.  Fix issues that might come out of that
* Working with Customer Success on addressing any `Outage` specific epics
* Building pipeline, provisioning automation work that may be needed
* The chance for the developer to improve on various issues and problems he or she has seen as a developer, this could include things like fixing up docker-compose, improving the docker deploys, improving code coverage, adding more Runscope/GhostInspector tests.

Schedule listed [here](https://docs.google.com/spreadsheets/d/12d391UI6M_XgzUhdzK1K4F-ESwMZb2LfN3-FWBIA0lI/edit#gid=0)
