Welcome to Synq.fm's R&D team, This is your one stop shop for getting to values, system, tools, processes and technology better.

*NOTE : This workspace is always changing to reflect our latest practices and technologies*

## Our Mission

Be the easiest and fastest way to integrate video technology/content into your app or service

## Core Behaviors

 * __Work as a team__ - collaborate together, no silos, no finger pointing, no blame culture.  Also, have fun and enjoy each other's time once in a while.  *We succeed or fail together*

 * __Execute Quickly, Improve constantly__ - Get things done quickly, and be vigilant about constant improvement.  *Don't be afraid of "failure"*

 * __Care about your craft__ - Add tests as you see fit, care about quality and correctness, be consistent, follow standards, add documentation.  *The little things matter*

## Getting Started :)

* Get Access to [Trello](https://trello.com/synq) - This is the tool Product Management uses to track features and milestones
 * Review our [Product Roadmap](https://trello.com/b/2YvamUq6/product-roadmap) trello board
 * Review our [Business Overview](https://trello.com/b/r0MwBrn2/synq-getting-started) trello board
* Get Acccess to and review API design on [Stoplight](https://app.stoplight.io/) (or read our OAS [spec](https://github.com/SYNQfm/spec-documentation/tree/master/obaku-specification))
* Get Access to 1Password - password manager for various shared services
* Get Access to Slack - install Slack or use the web browser.  We are at [synqfm.slack.com](https://synqfm.slack.com)
* Get Access to GitHub - Our repo is at [https://github.com/SYNQfm](https://github.com/SYNQfm)

### Getting started for non-employees

* Get access to our [Synq Hiring](https://join.slack.com/t/synq-hiring/shared_invite/enQtMjc5MjQ5NTg1ODExLWVhNWYxOTY0OTQ1M2JiZDBlZWJiMGViN2JmZGMyMTMzZWQxY2ExOGMyMTM3YzU2ZGRiZWMzZWVlYWY4ODkyMjQ) Slack team
* Review [Mini Projects](https://trello.com/b/YmdoqTFZ/mini-projects) that you'd like to work on
* Read our online [API docs](https://synq.api-docs.io/1.9.1/video-apis)
* Review our open source [SDKs](https://github.com/SYNQfm?utf8=%E2%9C%93&q=SYNQ%20sdk&type=&language=)
* Look at our [gosample](https://github.com/SYNQfm/gosample.git) app to see how we structure certain things


## Give me the code!!

__Core Services__

Name                                                        | Build | Code Coverage | Description  |  Maintainer(s) | Wiki Link
:-----------------------------------------------------------|------ | ------------- | ------------ | -------------- | -----------
[Akka](https://github.com/SYNQfm/akka)  | [![CircleCI](https://circleci.com/gh/SYNQfm/akka.svg?style=svg&circle-token=e19e0a215871658959ea60b8c5151e497241ba18)](https://circleci.com/gh/SYNQfm/akka) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/akka/badge.svg?t=gSJeot)](https://coveralls.io/github/SYNQfm/akka) | V2 API Core | Mike, Bruce | [here](https://github.com/SYNQfm/akka/wiki)
[Wraith](https://github.com/SYNQfm/wraith) | [![CircleCI](https://circleci.com/gh/SYNQfm/wraith.svg?style=svg&circle-token=40d1dd3788a0b3d067e84d124e96d5bbdeaaf139)](https://circleci.com/gh/SYNQfm/wraith) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/wraith/badge.svg?branch=master&t=uVtpKG)](https://coveralls.io/github/SYNQfm/wraith?branch=master) | V2 Webhooks  | Mike, Bruce | [here](https://github.com/SYNQfm/wraith/wiki)
[Unicorn](https://github.com/SYNQfm/unicorn) | [![CircleCI](https://circleci.com/gh/SYNQfm/unicorn.svg?style=svg&circle-token=0690b087ca33c31694a3dcea2d9e4bf9a04df3a2)](https://circleci.com/gh/SYNQfm/unicorn) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/unicorn/badge.svg?branch=master&t=u0kNmw)](https://coveralls.io/github/SYNQfm/unicorn?branch=master) | V2 Uploader service that will upload anything | Jessica | [here](https://github.com/SYNQfm/unicorn/wiki)
[Hydra](https://github.com/SYNQfm/hydra)            | [![CircleCI](https://circleci.com/gh/SYNQfm/hydra.svg?style=svg&circle-token=3bb209f5fceb013cfe5bdffed8867fb84693c789)](https://circleci.com/gh/SYNQfm/hydra) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/hydra/badge.svg?t=xMnp9a)](https://coveralls.io/github/SYNQfm/hydra) | Transcode jobs service | Bruce | [here](https://github.com/SYNQfm/hydra/wiki)
[Pixie](https://github.com/SYNQfm/pixie)           | [![CircleCI](https://circleci.com/gh/SYNQfm/pixie.svg?style=svg&circle-token=48d2d9d54880593f3335c5f07752fca21a514ef8)](https://circleci.com/gh/SYNQfm/pixie) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/pixie/badge.svg?t=njYMm6)](https://coveralls.io/github/SYNQfm/pixie) | Videojs player service | Jessica | [here](https://github.com/SYNQfm/pixie/wiki)
[Monopod](https://github.com/SYNQfm/monopod)           | | | Public Schedule 2/4 Metadata parser | Josh | [here](https://github.com/SYNQfm/monopod/wiki)


__Processing Services__

Name                                                        | Build | Code Coverage | Description  |  Maintainer(s) | Wiki Link
:-----------------------------------------------------------|------ | ------------- | ------------ | -------------- | -----------
[Ifrit](https://github.com/SYNQfm/ifrit) | [![CircleCI](https://circleci.com/gh/SYNQfm/ifrit.svg?style=svg&circle-token=c4b769d9df0c236f89eb90a4e5413307a152665f)](https://circleci.com/gh/SYNQfm/ifrit) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/ifrit/badge.svg?t=izPz3O)](https://coveralls.io/github/SYNQfm/ifrit) | Import large amount of files from disk | Bruce | [here](https://github.com/SYNQfm/ifrit/wiki)
[Charybdis](https://github.com/SYNQfm/charybdis) | [![CircleCI](https://circleci.com/gh/SYNQfm/charybdis.svg?style=svg&circle-token=07d34336bd24df048b532ed90e2b0b9cf9fea46c)](https://circleci.com/gh/SYNQfm/charybdis)| [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/charybdis/badge.svg?t=cuzDts)](https://coveralls.io/github/SYNQfm/charybdis) | CDN log store | Jessica | [here](https://github.com/SYNQfm/charybdis/wiki)
[Calingi](https://github.com/SYNQfm/calingi) | [![CircleCI](https://circleci.com/gh/SYNQfm/calingi.svg?style=svg&circle-token=35f2b9d5ba20859dfee3af32129b8f746645f665)](https://circleci.com/gh/SYNQfm/calingi)| [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/calingi/badge.svg?t=AgvRqu)](https://coveralls.io/github/SYNQfm/calingi) | CDN log parse | Jessica | [here](https://github.com/SYNQfm/calingi/wiki)
[Aerico](https://github.com/SYNQfm/aerico) | [![CircleCI](https://circleci.com/gh/SYNQfm/aerico.svg?style=svg&circle-token=6bf28fed9b7e034017e2c7229049f774b3e80bc3)](https://circleci.com/gh/SYNQfm/aerico) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/aerico/badge.svg?t=Go4IJe)](https://coveralls.io/github/SYNQfm/aerico) | Imports V1 Videos to V2 | Bruce | [here](https://github.com/SYNQfm/aerico/wiki)
[Anansi](https://github.com/SYNQfm/anansi) | [![CircleCI](https://circleci.com/gh/SYNQfm/anansi.svg?style=svg&circle-token=85d81001ef156fe3d431b47181bcc8bfa27bfb57)](https://circleci.com/gh/SYNQfm/anansi) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/anansi/badge.svg?t=QZb3mG)](https://coveralls.io/github/SYNQfm/anansi) | Metadata / Video quality analsysi tool | Shan | [here](https://github.com/SYNQfm/anansi/wiki)

__Frontend__

Name                                                        | Build | Code Coverage | Description  |  Maintainer(s) | Wiki Link
:-----------------------------------------------------------|------ | ------------- | ------------ | -------------- | -----------
[Doppelganger](https://github.com/SYNQfm/doppelganger) | | | ReactJS based Dashboard for SYNQ | Josh | [here](https://github.com/SYNQfm/doppelganger/wiki)
[Synq UI](https://github.com/SYNQfm/synq-ui) | | | Re-usable ReactJS components | Josh | [here](https://github.com/SYNQfm/synq-ui/wiki) 
[Wyvern](https://github.com/SYNQfm/wyvern) | | | This is a Wordpress site for www.synq.fm | Josh | [here](https://github.com/SYNQfm/wyvern/wiki)


__Ops Services__
 
Name                                                         | Description  |  Maintainer(s) |  Wiki Link  
:----------------------------------------------------------- | ------------ | -------------- | ----------- 
[Manticore](https://github.com/SYNQfm/manticore) | Lambda monitoring script(s)  | Josh, Glen  | [here](https://github.com/SYNQfm/manticore/wiki) 
[Imp](https://github.com/SYNQfm/imp) | DNS, Ansible | Glen, Bruce | [here](https://github.com/SYNQfm/imp/wiki) 

__Legacy Services__

Name                                                         | Build | Description  |  Maintainer(s)
:-----------------------------------------------------------|------ | ------------ | --------------
[Core](https://github.com/SYNQfm/obaku)                 | [![CircleCI](https://circleci.com/gh/SYNQfm/obaku.svg?style=svg&circle-token=9b25c63acb32232a9a7f9da2fa7240919d335cb0)](https://circleci.com/gh/SYNQfm/obaku)   | Main service including our APIs, datastore, query and webhook execution engine.                | Bruce
[Tylwythteg](https://github.com/SYNQfm/tylwythteg)      |     | Thumbnail generator service | Jessica
[Streamer](https://github.com/SYNQfm/streamer) | [![CircleCI](https://circleci.com/gh/SYNQfm/streamer.svg?style=svg&circle-token=b5519ed34ec02fcaa30e6b61c2098d7b0f3fd571)](https://circleci.com/gh/SYNQfm/streamer)               | Handles live streaming | Bruce
[Infrastructure](https://github.com/SYNQfm/obaku/infrastructure) |    | Previous Ansible, automation tools, currently lives in "Core" | Bruce
[File States](https://github.com/SYNQfm/obaku/file-states) |       | S3 Upload queue processing, currently lives in "Core" | Bruce
[Uploader V1](https://github.com/SYNQfm/obaku/uploader)|          | Uploader and multi-part signing, currently lives in "Core" | Jessica

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
* Cleanup Thursdays - set aside half a day per week for owners to fix various things, clean up workspaces/readmes, conduct code reviews etc.  Key is to STOP WHAT YOU'RE DOING and take the time to breathe and do some much needed cleanup :)

### Scheduling and Tracking work

* [Trello Roadmap](https://trello.com/b/2YvamUq6/product-roadmap) - This is where we track high level things to work on.  Business decides on key features and R&D will review those and assign developers to own a "card", which will then produce n issues in GitHub.  Dev will also add to the roadmap as well.
* GitHub Issues - specific work needed to accomplish and are usually tied to a Trello card.  We'll also have one off bugs, devop tasks, cleanup etc that is required for routine maintenance
* Once cards are assigned, each owner will be in charge of creating the issues needed to implement the card, so everything is driven by the owner.  Cards would be assigned based on the code it touches and who maintains and the time that person has.

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

### Supporting customers

* We use [Zendesk](https://synqsupport.zendesk.com) for support email, [Chatlio](https://chatlio.com/) for chat support and our [community](https://community.synq.fm) forum for forum based support.   Notifications for support tickets are sent to the #zendesk Slack channel and to Pagerduty if a support ticket is open for more than 2 hours. Notifications for chat support requests are sent to the #chatliosupport Slack channel. 
* In addition to the support channels mentioned, we use the [synq-onboarding](https://onboarding.synq.fm/) slack channel to help customers while they are onboarding and [Gitter.im](https://gitter.im/SYNQfm/Lobby) for any questions on our services from developers.
* The customer success team will handle initial requests but any one can chip into issues and help to resolve customer problems. 
* There is no Synq without customers and the customer success team is the eyes and ears of our customers and their requests should be taken seriously!


## Be kind, Rewind!

Here are some best practices for various topics

__Branching / PRs__

* Use good naming convention such as `bruce-fix-s3-bug`
* Strive for atomic changes per branch, try to limit it to 2 fixes max
* PRs should have
  * An issue attached, unless its a minor fix
  * Passing tests that covers relevant parts of the code (should be enforced by CI)
  * Minimum one person tagged to review the code
* PR Reviews should
  * Be short and usually take less than an hour
  * Cleared out quickly to avoid a pile up
  * Be reviewed within a day, otherwise the issuer can merge it without an approval
* "Squash and Merge" branches into master, and its a good habit to delete the merged branch at that time
  * If you need to see the commit history, it can be found in the original PR ( ex: [PR 6](https://github.com/SYNQfm/obaku/pull/6) )
* Maintain as few personal branches as possible
* More complicated workspaces should include a PR [template](https://github.com/SYNQfm/obaku/blob/master/.github/PULL_REQUEST_TEMPLATE.md)
* should pass the coveralls code coverage & unit tests (you can adjust the coveralls code coverage thresholds here https://coveralls.io/github/SYNQfm/obaku/settings. Note, this is just for the 'obaku' repositories, and assumes you have the correct access privileges to make changes!)

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
