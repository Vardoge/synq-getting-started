Welcome to Synq.fm's R&D team, This is your one stop shop for getting to values, system, tools, processes and technology better.

*NOTE : This workspace is always changing to reflect our latest practices and technologies*

## Our Values

 * __Team Mindset__ - collaborate together, no silos, no finger pointing, no blame culture.  Also, have fun and enjoy each other's time once in a while.  *We succeed or fail together*
 
 * __Execute Quickly, Improve constantly__ - Get things done quickly, and be vigilant about constant improvement.  *Don't be afraid of "failure"*

 * __Care about your craft__ - Add tests as you see fit, care about quality and correctness, be consistent, follow standards.  *The little things matter*
 

## Development Philosphy

We use a weekly delivery model here, organized by monthly milestones (more detail below).  The idea here is, we have a milestone with some key high level points, then break it down to digestable weekly deliverables, and then push code to production every week.

## Simple Guidelines

Here are some useful guidelines pertaining to our dev cycle, from issue management, to deploy, to repo and code review process.

__Issue tracker__    
[Issue Lifecycle](issue_tracker/README.md)    
[Issue Creation Guidelines](issue_tracker/guidelines.md)

__Monday dev meeting__    
[Agenda / purpose](issue_tracker/README.md)

__Deploy Guideline__

* Releases are tagged and finalized on mondays during/after dev meeting 14.30 GMT+1
* Deploy to production happens every Tuesday at 16:00 GMT+1
* A release should be created to a deploy to track the specific change pushed out
* Deploys should be done with scripts and avoid manual intervention or work
* Out of band deploys should only happen for critical outages or major security holes
* Anyone should be able to deploy
* Our goal is continuous deployment and moving the deploys to monday as they get leaner

__Repo Guidelines__

* Branch names should include first name of user
* Create a branch for each issue, and make it as "atomic" as possible.  Don't combine multiple features into a single branch
* Maintain no more than 1-2 active branches
* Always deploy from/branch from master

__PR Guidelines__

* PRs are posted to General
* PRs should reference a GitHub issue (only exception is for minor doc/test fixes)
* PR requests should not be open longer than a day.
* PR request reviews should focus on
 * Having Tests
 * Contain atomic changes
 * Code organized properly
 * Tests passed (is enforced)
 * Approved by a reviewer (is enforced)
* PR should be "Squash and Merged" and the branch deleted.  All commit history can be found in the PR for historical purposes ( ex: [PR 6](https://github.com/SYNQfm/obaku/pull/6) )

## Setup

* Get Access to Slack - install Slack or use the web browser.  We are at [synqfm.slack.com](https://synqfm.slack.com)
* Get Access to GitHub - Our repo is at [https://github.com/SYNQfm](https://github.com/SYNQfm)
* Get Access to Zenhub - This is a tool that sits on top of GitHub.   You will need a license where you can request one on Slack, and install the plugin [here]([here](https://chrome.google.com/webstore/detail/zenhub-for-github/ogcgkffhplmphkaahpmffcafajaocjbd?hl=en-US))

## Repositories

[Obaku](https://github.com/SYNQfm/obaku): Our main service, currently all the "microservices" are inside this one repo.    
[Synq Web Assets](https://github.com/SYNQfm/synq-web-assets.git): This is where our documentation, API specification etc are hosted.    
[Synq Website](https://github.com/SYNQfm/obaku/wordpress): This is a Wordpress site, which currently lives in the main repo.    
[Streamer](https://github.com/SYNQfm/streamer): Our first standalone micro-service to handle live streaming

## Resources

[Wiki](https://github.com/SYNQfm/obaku/wiki)    
[Continuous Improvement Board](https://trello.com/b/dv0Cpcmo/continuous-improvement)   
[Links](links.md)    
[Previous Dev Cycle Chart](dev_cycle.png)
