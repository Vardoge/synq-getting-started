Welcome to Synq.fm's R&D team, This is your one stop shop for getting to values, system, tools, processes and technology better.

*NOTE : This workspace is always changing to reflect our latest practices and technologies*

## Our Mission

Be the easiest and fastest way to integrate video technology/content into your app or service

## Core Behaviors

Concepts borrowed from Patreon's [culture](https://patreonhq.com/how-to-build-culture-that-lasts-dc25b086cefd) doc

 * __Work as a team__ - collaborate together, no silos, no finger pointing, no blame culture.  Also, have fun and enjoy each other's time once in a while.  *We succeed or fail together*
 
 * __Execute Quickly, Improve constantly__ - Get things done quickly, and be vigilant about constant improvement.  *Don't be afraid of "failure"*

 * __Care about your craft__ - Add tests as you see fit, care about quality and correctness, be consistent, follow standards, add documentation.  *The little things matter*

## Getting Started :)

* Get Access to 1Password - password manager for various shared services
* Read our online [API docs](api.synq.fm/docs)
* Get Acccess to and review API design on [Stoplight](https://app.stoplight.io/)
* Get Access to Slack - install Slack or use the web browser.  We are at [synqfm.slack.com](https://synqfm.slack.com)
* Get Access to GitHub - Our repo is at [https://github.com/SYNQfm](https://github.com/SYNQfm)
* Get Access to Zenhub - This is a tool that sits on top of GitHub.   You will need a license where you can request one on Slack, and install the plugin [here]([here](https://chrome.google.com/webstore/detail/zenhub-for-github/ogcgkffhplmphkaahpmffcafajaocjbd?hl=en-US))
* Reivew our open source [SDKs](https://github.com/SYNQfm?utf8=%E2%9C%93&q=SYNQ%20sdk&type=&language=)

## Give me the code!!

 Name                                                         | Description  |  Maintainer(s)
 :----------------------------------------------------------- | ------------ | --------------
 [Core](https://github.com/SYNQfm/obaku)                      | Our core service, contains our data store, APIs, query and webhook execution engine.  This also contains misc services required to run api.synq.fm. |  Martin, Bruce
 [Transcode](https://github.com/SYNQfm/hydra)                 | Transcode jobs service | Bruce
 [Player](https://github.com/SYNQfm/ballivian)                | Videojs player service | Srod
 [Thumbnails](https://github.com/SYNQfm/tylwythteg)           | Thumbnail generator service | Srod
 [Metadata](https://github.com/SYNQfm/monopod)                | Public Schedule 2/4 Metadata parser | Halvard
 [Importer](https://github.com/SYNQfm/importer)               | Import large amount of files from disk | Julian
 [Streamer](https://github.com/SYNQfm/streamer)               | Handles live streaming | Bruce
 [Core V2](https://github.com/SYNQfm/aerico)                  | Service to support proposed [V2](https://github.com/SYNQfm/obaku/wiki/Design:-Video-object-design-(present-&-future)) of our API | Julian, Martin
 [Synq Website](https://github.com/SYNQfm/obaku/wordpress)    | This is a Wordpress site, which currently lives in "Core" repo. | Halvard
 [Legacy Docs](https://github.com/SYNQfm/synq-web-assets.git) | This is where our documentation, API specification etc are hosted. | Srod

Note : Naming scheme looks at [creatures](https://en.wikipedia.org/wiki/Lists_of_legendary_creatures), ideally matching the same first few letters of the service "Thumbnails -> Tylwythteg"
 
## Software Development Lifecycle

### How we track work

* GitHub Milestones - created for each project, shoudl be 3-5 weeks long
* Zenhub "Epics" - created as high level place holders in the milestones
* GitHub Issues - specific work needed to accomplish epics and achieve our goal in the milestones.  Also can be one off bugs, devop tasks, cleanup etc that is required for routine maintenance

### How we schedule work

* Issues are all self scheduled.  Use the "Selected for dev" and "In progress" zenhub pipelines to manage your own workload
* Epics are created and scheduled during each Milestone Kick off meeting

### How we communicate

* Daily "Standups" on Slack via Geekbot (#standup channel)
* Via Slack primarily in #general or #developers
* Weekly Dev Meetings
 * Review Epics and Progress of Milestone
 * Go over "Help Wanted" issues
 * Discuss any major architecture decisions, changes, concerns
* Milestone Kickoff Meeting
 * Discuss "theme" of the milestone and schedule high level epics and assign them to developers

### How we test / deploy

* Use CircleCI for Continous Integration
* Use Coveralls to monitor test coverage
* Aim for continuous deployment.  Each repo maintainer determines the schedule of the deployments but should be no longer than 1 week (unless no changes were made)

## Best Practices

Below is some good best practices for getting the most out of your time

__Branching / PR__

* Use good naming convention such as `bruce-fix-s3-bug`
* Strive for atomic changes per branch, try to limit it to 2 fixes max
* PRs should reference an issue (unless its minor fixes)
* Maintain as few personal branches as possible
* Keep the number of open PRs low.
 * Before starting your work, do you notice a pile up of PRs?  Chip in and help clear it out!
* PRs should have
 * Passing tests (is enforced)
 * Minimum code coverage (is enforced)
 * Reviewed by at least one person (is enforced)
*  Be "Squash and Merged" and the branch deleted.  All commit history can be found in the PR for historical purposes ( ex: [PR 6](https://github.com/SYNQfm/obaku/pull/6) )

__Meetings__

* Should come with an agenda, the organizer should keep it focused
* Keep it as short as possible
* Think if you could do this over slack?  If so, why call the meeting?

## Resources

[Wiki](https://github.com/SYNQfm/getting-started/wiki)    
[Technologies to Explore](https://github.com/SYNQfm/getting-started/wiki/Technologies-to-Explore) - if you read something cool, put it here   
[Links](links.md)    
[Previous Dev Cycle Chart](dev_cycle.png)
