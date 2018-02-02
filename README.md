Welcome to Synq.fm's R&D team. This is your one stop shop for getting to values, system, tools, processes and technology better.

*NOTE : This workspace is always changing to reflect our latest practices and technologies*

## Our Mission

Be the fastest, most cost effective way to connect licensed video content between owners/licensors and distributors.

## Core Behaviors

 * __Work as a team__ - collaborate together, no silos, no finger pointing, no blame culture.  Also, have fun and enjoy each other's time once in a while.  *We succeed or fail together*

 * __Execute Quickly, Improve constantly__ - Get things done quickly and be vigilant about constant improvement.  *Don't be afraid of "failure"*

 * __Care about your craft__ - Add tests as you see fit, care about quality and correctness, be consistent, follow standards, add documentation.  *The little things matter*

## Getting Started :)

* Get Access to [Trello](https://trello.com/synq) - This is the tool Business and Development use to track high level work
  * Review [Dev Roadmap](https://trello.com/b/2YvamUq6/dev-roadmap) board
  * Review [Dev Team Info](https://trello.com/b/ShiJG8T8/dev-team-info) board
* Get Access to and review API design on [Stoplight](https://app.stoplight.io/) (or read our OAS [spec](https://github.com/SYNQfm/spec-documentation/tree/master/obaku-specification))
* Get Access to [Slack](https://synqfm.slack.com)
* Get Access to [GitHub](https://github.com/SYNQfm)
* Get Access to 1Password - password manager for various shared services

### For non-employees

* Get access to our [Synq Hiring](https://join.slack.com/t/synq-hiring/shared_invite/enQtMjc5MjQ5NTg1ODExLWVhNWYxOTY0OTQ1M2JiZDBlZWJiMGViN2JmZGMyMTMzZWQxY2ExOGMyMTM3YzU2ZGRiZWMzZWVlYWY4ODkyMjQ) Slack team
* Review [Mini Projects](https://trello.com/b/YmdoqTFZ/mini-projects) that you'd like to work on

## Give me the code!!

__Core Services__

Name                                                        | Build | Code Coverage | Description  |  Maintainer(s) | Wiki Link
:-----------------------------------------------------------|------ | ------------- | ------------ | -------------- | -----------
[Akka](https://github.com/SYNQfm/akka)  | [![CircleCI](https://circleci.com/gh/SYNQfm/akka.svg?style=svg&circle-token=e19e0a215871658959ea60b8c5151e497241ba18)](https://circleci.com/gh/SYNQfm/akka) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/akka/badge.svg?t=gSJeot)](https://coveralls.io/github/SYNQfm/akka) | V2 API Core | Mike, Bruce | [here](https://github.com/SYNQfm/akka/wiki)
[Wraith](https://github.com/SYNQfm/wraith) | [![CircleCI](https://circleci.com/gh/SYNQfm/wraith.svg?style=svg&circle-token=40d1dd3788a0b3d067e84d124e96d5bbdeaaf139)](https://circleci.com/gh/SYNQfm/wraith) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/wraith/badge.svg?branch=master&t=uVtpKG)](https://coveralls.io/github/SYNQfm/wraith?branch=master) | V2 Webhooks  | Mike, Bruce | [here](https://github.com/SYNQfm/wraith/wiki)
[Unicorn](https://github.com/SYNQfm/unicorn) | [![CircleCI](https://circleci.com/gh/SYNQfm/unicorn.svg?style=svg&circle-token=0690b087ca33c31694a3dcea2d9e4bf9a04df3a2)](https://circleci.com/gh/SYNQfm/unicorn) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/unicorn/badge.svg?branch=master&t=u0kNmw)](https://coveralls.io/github/SYNQfm/unicorn?branch=master) | V2 Uploader service that will upload anything | Jessica | [here](https://github.com/SYNQfm/unicorn/wiki)
[Hydra](https://github.com/SYNQfm/hydra)            | [![CircleCI](https://circleci.com/gh/SYNQfm/hydra.svg?style=svg&circle-token=3bb209f5fceb013cfe5bdffed8867fb84693c789)](https://circleci.com/gh/SYNQfm/hydra) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/hydra/badge.svg?t=xMnp9a)](https://coveralls.io/github/SYNQfm/hydra) | Transcode jobs service | Bruce | [here](https://github.com/SYNQfm/hydra/wiki)
[Pixie](https://github.com/SYNQfm/pixie)           | [![CircleCI](https://circleci.com/gh/SYNQfm/pixie.svg?style=svg&circle-token=48d2d9d54880593f3335c5f07752fca21a514ef8)](https://circleci.com/gh/SYNQfm/pixie) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/pixie/badge.svg?t=njYMm6)](https://coveralls.io/github/SYNQfm/pixie) | Videojs player service | Jessica | [here](https://github.com/SYNQfm/pixie/wiki)
[Monopod](https://github.com/SYNQfm/monopod)           | ![CircleCI](https://circleci.com/gh/SYNQfm/monopod/tree/master.svg?style=svg&circle-token=c18f5508984072ffde683c71cfde2fcb6e7fbc29) | | Public Schedule 2/4 Metadata parser | Josh | [here](https://github.com/SYNQfm/monopod/wiki)
[Ibong Adarna](https://github.com/SYNQfm/ibong-adarna) | | | Insights Services | Jessica |

__Processing Services__

Name                                                        | Build | Code Coverage | Description  |  Maintainer(s) | Wiki Link
:-----------------------------------------------------------|------ | ------------- | ------------ | -------------- | -----------
[Ifrit](https://github.com/SYNQfm/ifrit) | [![CircleCI](https://circleci.com/gh/SYNQfm/ifrit.svg?style=svg&circle-token=c4b769d9df0c236f89eb90a4e5413307a152665f)](https://circleci.com/gh/SYNQfm/ifrit) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/ifrit/badge.svg?t=izPz3O)](https://coveralls.io/github/SYNQfm/ifrit) | Import large amount of files from disk | Bruce | [here](https://github.com/SYNQfm/ifrit/wiki)
[Charybdis](https://github.com/SYNQfm/charybdis) | [![CircleCI](https://circleci.com/gh/SYNQfm/charybdis.svg?style=svg&circle-token=07d34336bd24df048b532ed90e2b0b9cf9fea46c)](https://circleci.com/gh/SYNQfm/charybdis)| [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/charybdis/badge.svg?t=cuzDts)](https://coveralls.io/github/SYNQfm/charybdis) | CDN log store | Jessica | [here](https://github.com/SYNQfm/charybdis/wiki)
[Calingi](https://github.com/SYNQfm/calingi) | [![CircleCI](https://circleci.com/gh/SYNQfm/calingi.svg?style=svg&circle-token=35f2b9d5ba20859dfee3af32129b8f746645f665)](https://circleci.com/gh/SYNQfm/calingi)| [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/calingi/badge.svg?t=AgvRqu)](https://coveralls.io/github/SYNQfm/calingi) | CDN log parse | Jessica | [here](https://github.com/SYNQfm/calingi/wiki)
[Aerico](https://github.com/SYNQfm/aerico) | [![CircleCI](https://circleci.com/gh/SYNQfm/aerico.svg?style=svg&circle-token=6bf28fed9b7e034017e2c7229049f774b3e80bc3)](https://circleci.com/gh/SYNQfm/aerico) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/aerico/badge.svg?t=Go4IJe)](https://coveralls.io/github/SYNQfm/aerico) | Imports V1 Videos to V2 | Bruce | [here](https://github.com/SYNQfm/aerico/wiki)
[Anansi](https://github.com/SYNQfm/anansi) | [![CircleCI](https://circleci.com/gh/SYNQfm/anansi.svg?style=svg&circle-token=85d81001ef156fe3d431b47181bcc8bfa27bfb57)](https://circleci.com/gh/SYNQfm/anansi) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/anansi/badge.svg?t=QZb3mG)](https://coveralls.io/github/SYNQfm/anansi) | Metadata / Video quality analysis tool | Shan | [here](https://github.com/SYNQfm/anansi/wiki)

__Frontend__

Name                                                        | Build | Code Coverage | Description  |  Maintainer(s) | Wiki Link
:-----------------------------------------------------------|------ | ------------- | ------------ | -------------- | -----------
[Duwende](https://github.com/SYNQfm/duwende) | | | ReactJS based Dashboard for SYNQ | Fiona, Josh | 
[Harpy](https://github.com/SYNQfm/harpy) | | | Static HTML Homepage | Josh | |

__Ops Services__
 
Name                                                         | Description  |  Maintainer(s) |  Wiki Link  
:----------------------------------------------------------- | ------------ | -------------- | ----------- 
[Manticore](https://github.com/SYNQfm/manticore) | Lambda monitoring script(s)  | Josh, Glen  | [here](https://github.com/SYNQfm/manticore/wiki) 
[Imp](https://github.com/SYNQfm/imp) | DNS, Ansible | Glen, Bruce | [here](https://github.com/SYNQfm/imp/wiki) 

__Legacy Services__

Name                                                         | Build | Description  |  Maintainer(s)
:-----------------------------------------------------------|------ | ------------ | --------------
[Tylwythteg](https://github.com/SYNQfm/tylwythteg)      |     | Thumbnail generator service | Jessica
[Infrastructure](https://github.com/SYNQfm/obaku/infrastructure) |    | Previous Ansible, automation tools, currently lives in "Core" | Bruce

Repo naming scheme is based on [legendary creatures](https://en.wikipedia.org/wiki/Lists_of_legendary_creatures), ideally matching the first (or more) letter(s) of the service "Thumbnails -> Tylwythteg"

## How we software ;)

### Maintaining code

* Each repo has a main maintainer and a co-owner that would be their backup.  We use the CODEOWNERS settings in GitHub to track this (first name is the main maintainer)
* The Main Maintainer is responsible for
  * Naming of the repo
  * Selecting the co-owner for that repo
  * Keep tests and code coverage high
  * Maintenance of the issues, README, and ensuring others can contribute to the repo easily (without the maintainer being there).
  * Ensuring proper PR reviews and periodic code reviews
  * Come up with ideas to improve the system, repo or process
* [Cleanup Thursdays](https://trello.com/b/ZI68fM9w/cleanup-thursdays) - Set aside half a day per week for owners to fix various things. The key is to STOP WHAT YOU'RE DOING and take the time to breathe and do some much needed cleanup :). Here's a small list of things that could be done:
  - clean up workspaces/readmes 
  - conduct code reviews
  - refactor
  - increase testing
  - fix all "#TODOS"
  
### Scheduling and Tracking work

* [Product Board](https://trello.com/b/obntC0BM/product-board) - High level requirements come into here and business and dev figure out what is possible, scope, and cards required.  This is where all the vetting goes and by the time it hits the development roadmap, most things are hashed out.
* [Dev Roadmap](https://trello.com/b/2YvamUq6/dev-roadmap) - This is where we track our milestones, epics and week to week tasks.
* GitHub Issues - specific work needed to accomplish and are usually tied to a Trello card

### Communicating

* Using Slack
  * Primarily in #general or #developers
  * Daily "Standups" via Geekbot (posted to #standup)
* [Weekly Dev Meetings](https://trello.com/b/ShiJG8T8/dev-meetings)
  * Review current status of Milestones
  * Discuss any issues/blockers concerning the team
  * Go over major features/architecture/design decisions
  * Review future milestones, planning and discussions
* Yearly Dev Summit Meeting
  * Time to get together and enjoy each other in real life
  * Intense 4 day planning sessions to go over key iniatitives for the new year
  
### Test / Deploy / Run

* We use [CircleCI](https://circleci.com/dashboard) for Continous Integration
* We use [Coveralls](https://coveralls.io/) to monitor test coverage
* Aim for continuous deployment. Maintainers determine the release cadence but changes _should_ be deployed at least once a week
  * Some services use [Heroku](https://dashboard.heroku.com/teams/synqfm/apps) with automatic deploys on changes to `master`
  * Some services use [Nanobox](https://dashboard.nanobox.io/)
* We use [Runscope](https://www.runscope.com/radar/si8c3oxplpmd) to continuously monitor our APIs 
* We use [PagerDuty](https://app.pagerduty.com/) to manage on call and alerts
* We use [StatusPage](https://manage.statuspage.io/pages/x9f990zglm69) to communicate public API [status](https://synq.statuspage.io/) information to customers

### Supporting Prospects/Customers

* We use [Zendesk](https://synqsupport.zendesk.com) for support email and the [synq-onboarding](https://synq-onboarding.slack.com) slack channel to help customers.
* We use Hubspot to track our customers and various interactions and converting our leads into signed deals.

## Be kind, Rewind!

Here are some best practices for various topics

__Branching / PRs__

* Use good naming convention such as `bruce-fix-s3-bug`
* Strive for atomic changes per branch, try to limit it to 2 fixes max
* PRs should have passing testing and good code coverage (>70%) before they are merged (these are usually enforced)
* "Squash and Merge" branches into master, and delete the merged branch at that time
* Delete unused branches, maintain as few working branches as possible

__Code Reviews__

* Anyone can nominate a code area to review, and the code owner would run the review
* Code reviews should take 1-3 hours and be done at one time
* We should do at most one review every 2 weeks

__Meetings__

* Should come with an agenda, the organizer should keep it focused
* Keep it as short as possible
* Think if you could do this over slack?  If so, why call the meeting?

## Resources

[Technologies to Explore](https://github.com/SYNQfm/getting-started/wiki/Technologies-to-Explore) - if you read something cool, put it here    
[Useful Links](links.md)    
[General Wiki](https://github.com/SYNQfm/getting-started/wiki)
