Welcome to Synq.fm's R&D team's getting started guide.  This document describes our development philosophy and the reasoning behind the way we do certain things and show very specific examples of how we live by our philosophy.  Anyone can suggest changes to this document, but its good to read this first to understand the why on our process

## Our Mission

`To deliver business value quickly and iteratively`

## How and why we do it

`Ship production code continuously`

In order to accomplish our goal, we do the below things.  Click on each item to see more details

What   | Reasoning | Tooling | Category
:------- | ----- | --------- | -------
[(Near) Atomic Changes](code.md) | Pushing smaller changes allows us to delivery incremental value, also reduces change of breakage | GitHub | Code
[High code coverage](code.md) | CI is useless without good quality coverage, and we can't ship to production confidently without it | CircleCI, Coveralls | Code
[Refactor constantly](devops.md) | Code debt slows us down and to counter our fast PR turnaround | GitHub | Code
[Branches and PRs](docs.md) | introduce small changes safely, ensure the code fits our philosophy, knowledge sharing | GitHub, Slack | Docs
[Good documentation](docs.md) | moving quickly means we work on a lot of different things, coming back to it later or having another teammmate look at it, they need to know | GitHub Markdown, Wiki, Stoplight | Docs
[Aligned Development](docs) | Make sure what we're working on brings business value | Trello, GitHub | Docs
[Tight CI/CD](devops.md) | The way we can ship the code quickly and confidently | GithHub, CircleCI, Nanobox + Digital Ocean or Heroku | DevOps
[Automated System/UI Testing](devops.md) | Once code is in production, is it really working?  Running things like Runscope against the API gives us confidence that new changes didn't mess up prod | CircleCI, Runscope, GhostInspector, TestLodge | DevOps
[DevOps Culture](devops.md) | Everyone should know how stuff runs and keep an eye that services are working as expected | Slack, Runscope, PagerDuty, StatusPages | DevOps

## Doing it right with Core Behaviors

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

## Technology Overview

[Architecture Diagram](https://trello.com/c/YofhnSkC/237-architecture-of-synq-media)

__Core Services__

Name                                                        | Build | Code Coverage | Description  |  Maintainer(s) | Wiki Link
:-----------------------------------------------------------|------ | ------------- | ------------ | -------------- | -----------
[Akka](https://github.com/SYNQfm/akka)  | [![CircleCI](https://circleci.com/gh/SYNQfm/akka.svg?style=svg&circle-token=e19e0a215871658959ea60b8c5151e497241ba18)](https://circleci.com/gh/SYNQfm/akka) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/akka/badge.svg?t=gSJeot)](https://coveralls.io/github/SYNQfm/akka) | API Core | Bruce, Mike | [here](https://github.com/SYNQfm/akka/wiki)
[Wraith](https://github.com/SYNQfm/wraith) | [![CircleCI](https://circleci.com/gh/SYNQfm/wraith.svg?style=svg&circle-token=40d1dd3788a0b3d067e84d124e96d5bbdeaaf139)](https://circleci.com/gh/SYNQfm/wraith) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/wraith/badge.svg?branch=master&t=uVtpKG)](https://coveralls.io/github/SYNQfm/wraith?branch=master) | Programmable Webhooks  | Josh, Bruce | [here](https://github.com/SYNQfm/wraith/wiki)
[Unicorn](https://github.com/SYNQfm/unicorn) | [![CircleCI](https://circleci.com/gh/SYNQfm/unicorn.svg?style=svg&circle-token=0690b087ca33c31694a3dcea2d9e4bf9a04df3a2)](https://circleci.com/gh/SYNQfm/unicorn) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/unicorn/badge.svg?branch=master&t=u0kNmw)](https://coveralls.io/github/SYNQfm/unicorn?branch=master) | Upload API producing s3 signed urls | Jessica | [here](https://github.com/SYNQfm/unicorn/wiki)
[Hydra](https://github.com/SYNQfm/hydra)            | [![CircleCI](https://circleci.com/gh/SYNQfm/hydra.svg?style=svg&circle-token=3bb209f5fceb013cfe5bdffed8867fb84693c789)](https://circleci.com/gh/SYNQfm/hydra) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/hydra/badge.svg?t=xMnp9a)](https://coveralls.io/github/SYNQfm/hydra) | Transcode jobs service | Bruce, Jessica | [here](https://github.com/SYNQfm/hydra/wiki)
[Pixie](https://github.com/SYNQfm/pixie)           | [![CircleCI](https://circleci.com/gh/SYNQfm/pixie.svg?style=svg&circle-token=48d2d9d54880593f3335c5f07752fca21a514ef8)](https://circleci.com/gh/SYNQfm/pixie) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/pixie/badge.svg?t=njYMm6)](https://coveralls.io/github/SYNQfm/pixie) | Videojs player service | Jessica, Bruce | [here](https://github.com/SYNQfm/pixie/wiki)
[Mizuchi](https://github.com/SYNQfm/mizuchi)           | [![CircleCI](https://circleci.com/gh/SYNQfm/wraith.svg?style=svg&circle-token=40d1dd3788a0b3d067e84d124e96d5bbdeaaf139)](https://circleci.com/gh/SYNQfm/wraith) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/mizuchi/badge.svg?branch=master&t=PAqpkU)](https://coveralls.io/github/SYNQfm/mizuchi?branch=master) | Media Metadata parser | Josh | [here](https://github.com/SYNQfm/monopod/wiki)

__Processing Services__

Name                                                        | Build | Code Coverage | Description  |  Maintainer(s) | Wiki Link
:-----------------------------------------------------------|------ | ------------- | ------------ | -------------- | -----------
[Ifrit](https://github.com/SYNQfm/ifrit) | [![CircleCI](https://circleci.com/gh/SYNQfm/ifrit.svg?style=svg&circle-token=c4b769d9df0c236f89eb90a4e5413307a152665f)](https://circleci.com/gh/SYNQfm/ifrit) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/ifrit/badge.svg?t=izPz3O)](https://coveralls.io/github/SYNQfm/ifrit) | Import large amount of files from disk | Bruce | [here](https://github.com/SYNQfm/ifrit/wiki)
[Charybdis](https://github.com/SYNQfm/charybdis) | [![CircleCI](https://circleci.com/gh/SYNQfm/charybdis.svg?style=svg&circle-token=07d34336bd24df048b532ed90e2b0b9cf9fea46c)](https://circleci.com/gh/SYNQfm/charybdis)| [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/charybdis/badge.svg?t=cuzDts)](https://coveralls.io/github/SYNQfm/charybdis) | CDN log store | Jessica | [here](https://github.com/SYNQfm/charybdis/wiki)
[Calingi](https://github.com/SYNQfm/calingi) | [![CircleCI](https://circleci.com/gh/SYNQfm/calingi.svg?style=svg&circle-token=35f2b9d5ba20859dfee3af32129b8f746645f665)](https://circleci.com/gh/SYNQfm/calingi)| [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/calingi/badge.svg?t=AgvRqu)](https://coveralls.io/github/SYNQfm/calingi) | CDN log parse | Jessica | [here](https://github.com/SYNQfm/calingi/wiki)
[Aerico](https://github.com/SYNQfm/aerico) | [![CircleCI](https://circleci.com/gh/SYNQfm/aerico.svg?style=svg&circle-token=6bf28fed9b7e034017e2c7229049f774b3e80bc3)](https://circleci.com/gh/SYNQfm/aerico) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/aerico/badge.svg?t=Go4IJe)](https://coveralls.io/github/SYNQfm/aerico) | CLI Cleanup, Legacy -> New importer | Bruce | [here](https://github.com/SYNQfm/aerico/wiki)
[Anansi](https://github.com/SYNQfm/anansi) | [![CircleCI](https://circleci.com/gh/SYNQfm/anansi.svg?style=svg&circle-token=85d81001ef156fe3d431b47181bcc8bfa27bfb57)](https://circleci.com/gh/SYNQfm/anansi) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/anansi/badge.svg?t=QZb3mG)](https://coveralls.io/github/SYNQfm/anansi) | Metadata / Video quality analysis tool | Shan | [here](https://github.com/SYNQfm/anansi/wiki)
[Serpent](https://github.com/SYNQfm/serpent) | [![CircleCI](https://circleci.com/gh/SYNQfm/serpent.svg?style=svg&circle-token=72818c7c369b486bd9c73e132517731907e3e72e)](https://circleci.com/gh/SYNQfm/serpent) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/serpent/badge.svg?t=ztcRW1)](https://coveralls.io/github/SYNQfm/serpent) | Search Service | Shan |

__Frontend__

Name                                                        | Build | Code Coverage | Description  |  Maintainer(s) | Wiki Link
:-----------------------------------------------------------|------ | ------------- | ------------ | -------------- | -----------
[Duwende](https://github.com/SYNQfm/duwende) |[![CircleCI](https://circleci.com/gh/SYNQfm/duwende.svg?style=svg&circle-token=7824d007524d1618e7c8c702a6a2bdd7af0c914d)](https://circleci.com/gh/SYNQfm/duwende) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/duwende/badge.svg?branch=master&t=nBpAUi)](https://coveralls.io/github/SYNQfm/duwende?branch=master) | ReactJS based Dashboard for SYNQ | Fiona, Josh | 

__Ops Services__
 
Name                                                         | Description  |  Maintainer(s) |  Wiki Link  
:----------------------------------------------------------- | ------------ | -------------- | ----------- 
[Imp](https://github.com/SYNQfm/imp) | DNS, Ansible | Glen, Bruce | [here](https://github.com/SYNQfm/imp/wiki) 

Repo naming scheme is based on [legendary creatures](https://en.wikipedia.org/wiki/Lists_of_legendary_creatures), ideally matching the first (or more) letter(s) of the service "Search -> Serpent"

## Resources

[Technologies to Explore](https://github.com/SYNQfm/getting-started/wiki/Technologies-to-Explore) - if you read something cool, put it here    
[Useful Links](links.md)    
[General Wiki](https://github.com/SYNQfm/getting-started/wiki)
