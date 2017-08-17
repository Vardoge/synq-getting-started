Welcome to Synq.fm's R&D team, This is your one stop shop for getting to values, system, tools, processes and technology better.

*NOTE : This workspace is always changing to reflect our latest practices and technologies*

## Our Mission

Be the easiest and fastest way to integrate video technology/content into your app or service

## Core Behaviors

 * __Work as a team__ - collaborate together, no silos, no finger pointing, no blame culture.  Also, have fun and enjoy each other's time once in a while.  *We succeed or fail together*
 
 * __Execute Quickly, Improve constantly__ - Get things done quickly, and be vigilant about constant improvement.  *Don't be afraid of "failure"*

 * __Care about your craft__ - Add tests as you see fit, care about quality and correctness, be consistent, follow standards, add documentation.  *The little things matter*

## Getting Started :)

* Get Access to 1Password - password manager for various shared services
* Read our online [API docs](api.synq.fm/docs)
* Get Acccess to and review API design on [Stoplight](https://app.stoplight.io/) (or read our OAS [spec](https://github.com/SYNQfm/spec-documentation/tree/master/obaku-specification))
* Get Access to Slack - install Slack or use the web browser.  We are at [synqfm.slack.com](https://synqfm.slack.com)
* Get Access to GitHub - Our repo is at [https://github.com/SYNQfm](https://github.com/SYNQfm)
* Get Access to Zenhub - This is a tool that sits on top of GitHub.   You will need a license where you can request one on Slack, and install the [plugin](https://chrome.google.com/webstore/detail/zenhub-for-github/ogcgkffhplmphkaahpmffcafajaocjbd?hl=en-US))
* Reivew our open source [SDKs](https://github.com/SYNQfm?utf8=%E2%9C%93&q=SYNQ%20sdk&type=&language=)

## Give me the code!!

 Name                                                         | Description  |  Maintainer(s)
 :----------------------------------------------------------- | ------------ | --------------
 [Core](https://github.com/SYNQfm/obaku)                      | Main service including our APIs, datastore, query and webhook execution engine.                                                   |  Martin, Bruce
 [Transcode](https://github.com/SYNQfm/hydra)                 | Transcode jobs service | Bruce
 [Player](https://github.com/SYNQfm/ballivian)                | Videojs player service | Srod
 [Thumbnails](https://github.com/SYNQfm/tylwythteg)           | Thumbnail generator service | Srod
 [Metadata](https://github.com/SYNQfm/monopod)                | Public Schedule 2/4 Metadata parser | Halvard
 [Importer](https://github.com/SYNQfm/ifrit)                  | Import large amount of files from disk | Julian
 [Uploader](https://github.com/SYNQfm/obaku/uploader)         | Uploader and multi-part signing, currently lives in "Core" | Srod
 [File States](https://github.com/SYNQfm/obaku/file-states)      | S3 Upload queue processing, currently lives in "Core" | Martin
 [Streamer](https://github.com/SYNQfm/streamer)               | Handles live streaming | Bruce
 [Core V2](https://github.com/SYNQfm/aerico)                  | Service to support proposed [V2](https://github.com/SYNQfm/obaku/wiki/Design:-Video-object-design-(present-&-future)) of our API | Julian, Martin
 [Synq Website](https://github.com/SYNQfm/obaku/wordpress)    | This is a Wordpress site, which currently lives in "Core" | Halvard
 [Infrastructure](https://github.com/SYNQfm/obaku/infrastructure)    | DNS, Ansible, automation, currently lives in "Core" | Halvard
 [Legacy Docs](https://github.com/SYNQfm/synq-web-assets.git) | This is where our documentation, API specification etc are hosted. | Srod

Repo naming scheme is based on [legendary creatures](https://en.wikipedia.org/wiki/Lists_of_legendary_creatures), ideally matching the first (or more) letter(s) of the service "Thumbnails -> Tylwythteg"
 
## How we software

### How we track work

* GitHub Milestones - created for each project, should be 3-6 weeks long
* Zenhub "Epics" - created as high level place holders in the milestones.  Grouping for multiple issues.  These are also used to group outage information
* GitHub Issues - specific work needed to accomplish epics and achieve our goal in the milestones.  Also can be one off bugs, devop tasks, cleanup etc that is required for routine maintenance

### How we schedule work

* Epics are created and scheduled during each Milestone Kick off meeting
  * This should be used to group key functionality we want to implement
  * An owner will be assigned to an epic and it will be up to the owner to create the appropriate individual issues.
* Issues are self scheduled.  Use the "Selected for dev" and "In progress" zenhub pipelines to manage your own workload
  * Issues associated with Epics usually are higher priority
  * Issues to remediate outage problems should have higher priority (even overriding Epic work depending on severity)
* Issues can be created by anyone at the company
* Issues should be culled aggressively and if you don't think we're going to work on it in the next 3 months, you should just close it

### How we communicate

* Using Slack
  * Primarily in #general or #developers
  * Daily "Standups" via Geekbot (posted to #standup)
* Weekly Dev Meetings
  * Review Epics and Progress of Milestone
  * Go over "Help Wanted" issues
  * Discuss any major architecture decisions, changes, concerns
  * Review Outage Epics and schedule them accordingly
* Milestone Kickoff Meeting
  * Discuss "theme" of the milestone and schedule high level epics and assign them to developers

### How we test / deploy / run

* We use [CircleCI](https://circleci.com/dashboard) for Continous Integration
* We use [Coveralls](https://coveralls.io/) to monitor test coverage
* Aim for continuous deployment. Maintainers determine the release cadence but changes should be deployed at least once a week
  * Some services use [Heroku](https://dashboard.heroku.com/teams/synqfm/apps) with automatic deploys on changes to `master`
  * "Core" runs on DigitalOcean with a manual "tag and build" [deploy](deploy.md) model
* We use [Runscope](https://www.runscope.com/radar/si8c3oxplpmd) to continuously monitor our APIs
* We use [PagerDuty](https://app.pagerduty.com/) to manage on call and alerts
* We use [StatusPage](https://manage.statuspage.io/pages/x9f990zglm69) to communicate public API [status](https://synq.statuspage.io/) information to customers

### How we support our customers

* We use [Zendesk](https://synqsupport.zendesk.com) for support email and chat.  Notifications are sent to the #zendesk Slack channel
* The customer success team will handle initial requests but any one can chip into issues and help to resolve customer problems
* There is no Synq without customers and the customer success team is the eyes and ears of our customers and their requests should be taken seriously!

## Be kind, Rewind!

Below are some best practices for various topics

__Branching / PRs__

* Use good naming convention such as `bruce-fix-s3-bug`
* Strive for atomic changes per branch, try to limit it to 2 fixes max
* PRs should have
  * An issue attached, unless its a minor fix
  * Passing tests (is enforced)
  * Minimum code coverage (is enforced)
  * Minimum one person tagged to review the code
* PR Reviews should
  * Be short and usually take less than an hour
  * Cleared out quickly to avoid a pile up
  * Be reviewed within a day, otherwise the issuer can merge it without an approval
* "Squash and Merge" branches into master, and its a good habit to delete the merged branch at that time
  * If you need to see the commit history, it can be found in the original PR ( ex: [PR 6](https://github.com/SYNQfm/obaku/pull/6) )
* Maintain as few personal branches as possible
* More complicated workspaces should include a PR [template](https://github.com/SYNQfm/obaku/blob/master/.github/PULL_REQUEST_TEMPLATE.md)

__Code Reviews__

* Anyone can nominate a code area to review, and the code owner would run the review
* Code reviews should take 2-3 hours and be done at one time
* We should do at most one review every 2 weeks

__Meetings__

* Should come with an agenda, the organizer should keep it focused
* Keep it as short as possible
* Think if you could do this over slack?  If so, why call the meeting?

__Deploy__

* [Procedures](deploy.md) for repos that require a bit more manual work (ie Core)

## Resources

[Technologies to Explore](https://github.com/SYNQfm/getting-started/wiki/Technologies-to-Explore) - if you read something cool, put it here   
[Useful Links](links.md)    
[General Wiki](https://github.com/SYNQfm/getting-started/wiki)    