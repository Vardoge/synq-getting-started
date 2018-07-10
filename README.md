Welcome to Synq.fm's R&D team's getting started guide.  This document describes our development philosophy and outlines things we care about as a team.

## Our Mission

`To deliver business value quickly and iteratively`

## Doing it right with Core Behaviors

If you are on the Synq Engineering team you already exhibit some (or all) of these behaviors, but if you don't exhibit all, don't worry. We understand some of these behaviors rely on a bridge of trust, and we're happy to build that with you.

 * __Psychological Safety__ - It starts here, without Psychological Safety we cannot Communicate and we cannot Care. These are some examples of creating a psychologically safe team, everyone must be responsible and exhibit these behaviors at Synq. Some examples:
     * Encourage team mate participation.
     * Engage and investigate all ideas equally.
     * Define problems collectively as a group.
     * Make sure everyone has a chance to participate.
     * No blame, succeed or fail together mentality.
     * Willingness to try without fear.
     * For more details and examples read [here](https://en.wikipedia.org/wiki/Psychological_safety)
     

 * __Communication__ - Communication can take many forms, but it is important that we are always communicating at Synq. Without communication, none of this is possible. The only clause here is that we don't want to be jerks; if you are feeling upset please take time to construct your narrative before sharing it (see psychological safety). Some examples:
      * Creating PRs.
      * Writing documentation.
      * Communicating in person or online.
      * Giving and receiving feedback constructively and in real time
      
 * __Care about...__ - If you don't care about Synq, about your craft, about engineering, or about your coworkers, working here will be tough. You don't have to care about everything, but caring about something is important. Without caring you wouldn't be motivated to do the work that's required of you here. Some examples:
      * Care about Synq.
      * Care about your coworkers and their success.
      * Care about standards or quality.
      * Care about the craftmanship of your work.
      * Care about learning and growing your skills.

If you retain anything from this article, it is the 3 core behaviors from above.  We live by this, we hire by this, we fire by this.  You can review past hiring/firing decisions [here](https://trello.com/b/0Vb4DSJ0/hiring).

## How and why we do it

Here are things we specifically do to help achieve our mission

[__Code__](code.md)

What   | Reasoning | Tooling
:------- | ----- | ---------
(Near) Atomic Changes | Pushing smaller changes allows us to deliver incremental value; also reduces chance of breakage | GitHub
High code coverage | CI is useless without good quality coverage, and we can't ship to production confidently without it | CircleCI, Coveralls
Refactor constantly | Code debt slows us down and counters our fast PR turnaround | GitHub

[__Docs__](docs.md)

What   | Reasoning | Tooling
:------- | ----- | ---------
Branches and PRs | introduce small changes safely, ensure the code fits our philosophy, knowledge sharing | GitHub, Slack
Effective documentation | moving quickly means we work on a lot of different things, coming back to it later or having another teammmate look at it, they need to know | GitHub Markdown, StackOverflow, Stoplight
Aligned Development | Make sure what we're working on brings business value | Trello, GitHub

[__DevOps__](devops.md)

What   | Reasoning | Tooling
:------- | ----- | ---------
Tight CI/CD | The way we can ship the code quickly and confidently | GithHub, CircleCI, Nanobox + Digital Ocean or Heroku
Automated System/UI Testing | Once code is in production, is it really working?  Running things like Runscope against the API gives us confidence that new changes didn't mess up prod | CircleCI, Runscope, GhostInspector, TestLodge
DevOps Culture| Everyone should know how stuff runs and keep an eye that services are working as expected | Slack, Runscope, PagerDuty, StatusPages

## Technology Overview

[Architecture Diagram](https://trello.com/c/YofhnSkC/237-architecture-of-synq-media)

__Core Services__

Name                                                        | Build | Code Coverage | Description  |  Maintainer(s) | Wiki Link
:-----------------------------------------------------------|------ | ------------- | ------------ | -------------- | -----------
[Akka](https://github.com/SYNQfm/akka)  | [![CircleCI](https://circleci.com/gh/SYNQfm/akka.svg?style=svg&circle-token=e19e0a215871658959ea60b8c5151e497241ba18)](https://circleci.com/gh/SYNQfm/akka) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/akka/badge.svg?t=gSJeot)](https://coveralls.io/github/SYNQfm/akka) | API Core | Bruce, Fiona | [here](https://github.com/SYNQfm/akka/wiki)
[Wraith](https://github.com/SYNQfm/wraith) | [![CircleCI](https://circleci.com/gh/SYNQfm/wraith.svg?style=svg&circle-token=40d1dd3788a0b3d067e84d124e96d5bbdeaaf139)](https://circleci.com/gh/SYNQfm/wraith) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/wraith/badge.svg?branch=master&t=uVtpKG)](https://coveralls.io/github/SYNQfm/wraith?branch=master) | Programmable Webhooks  | Chris, Bruce | [here](https://github.com/SYNQfm/wraith/wiki)
[Unicorn](https://github.com/SYNQfm/unicorn) | [![CircleCI](https://circleci.com/gh/SYNQfm/unicorn.svg?style=svg&circle-token=0690b087ca33c31694a3dcea2d9e4bf9a04df3a2)](https://circleci.com/gh/SYNQfm/unicorn) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/unicorn/badge.svg?branch=master&t=u0kNmw)](https://coveralls.io/github/SYNQfm/unicorn?branch=master) | Upload API producing s3 signed urls | Bruce, Jessica | [here](https://github.com/SYNQfm/unicorn/wiki)
[Hydra](https://github.com/SYNQfm/hydra)            | [![CircleCI](https://circleci.com/gh/SYNQfm/hydra.svg?style=svg&circle-token=3bb209f5fceb013cfe5bdffed8867fb84693c789)](https://circleci.com/gh/SYNQfm/hydra) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/hydra/badge.svg?t=xMnp9a)](https://coveralls.io/github/SYNQfm/hydra) | Transcode jobs service | Bruce, Jessica | [here](https://github.com/SYNQfm/hydra/wiki)
[Pixie](https://github.com/SYNQfm/pixie)           | [![CircleCI](https://circleci.com/gh/SYNQfm/pixie.svg?style=svg&circle-token=48d2d9d54880593f3335c5f07752fca21a514ef8)](https://circleci.com/gh/SYNQfm/pixie) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/pixie/badge.svg?t=njYMm6)](https://coveralls.io/github/SYNQfm/pixie) | Videojs player service | Jessica, Bruce | [here](https://github.com/SYNQfm/pixie/wiki)
[Mizuchi](https://github.com/SYNQfm/mizuchi)           | [![CircleCI](https://circleci.com/gh/SYNQfm/wraith.svg?style=svg&circle-token=40d1dd3788a0b3d067e84d124e96d5bbdeaaf139)](https://circleci.com/gh/SYNQfm/wraith) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/mizuchi/badge.svg?branch=master&t=PAqpkU)](https://coveralls.io/github/SYNQfm/mizuchi?branch=master) | Media Metadata parser | Chris, Shan | [here](https://github.com/SYNQfm/monopod/wiki)

__Processing Services__

Name                                                        | Build | Code Coverage | Description  |  Maintainer(s) | Wiki Link
:-----------------------------------------------------------|------ | ------------- | ------------ | -------------- | -----------
[Ifrit](https://github.com/SYNQfm/ifrit) | [![CircleCI](https://circleci.com/gh/SYNQfm/ifrit.svg?style=svg&circle-token=c4b769d9df0c236f89eb90a4e5413307a152665f)](https://circleci.com/gh/SYNQfm/ifrit) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/ifrit/badge.svg?t=izPz3O)](https://coveralls.io/github/SYNQfm/ifrit) | Import large amount of files from disk | Bruce | [here](https://github.com/SYNQfm/ifrit/wiki)
[Incubus](https://github.com/SYNQfm/incubus) | [![CircleCI](https://circleci.com/gh/SYNQfm/incubus.svg?style=svg&circle-token=cbba819e2c1be4b1dcd2fbc9f99b9263bd67d78d)](https://circleci.com/gh/SYNQfm/incubus) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/incubus/badge.svg?t=sO2NOV)](https://coveralls.io/github/SYNQfm/incubus) | Lambda Importer | Jessica | [here](https://github.com/SYNQfm/incubus/wiki)
[Ikiryo](https://github.com/SYNQfm/ikiryo) | [![CircleCI](https://circleci.com/gh/SYNQfm/ikiryo.svg?style=svg&circle-token=f89c5eecedc55aa7a3e38522ace610db5bc3f6d5)](https://circleci.com/gh/SYNQfm/ikiryo) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/ikiryo/badge.svg?t=rRNMpE)](https://coveralls.io/github/SYNQfm/ikiryo) | Lambda Importer | Chris | [here](https://github.com/SYNQfm/ikiryo/wiki)
[Charybdis](https://github.com/SYNQfm/charybdis) | [![CircleCI](https://circleci.com/gh/SYNQfm/charybdis.svg?style=svg&circle-token=07d34336bd24df048b532ed90e2b0b9cf9fea46c)](https://circleci.com/gh/SYNQfm/charybdis)| [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/charybdis/badge.svg?t=cuzDts)](https://coveralls.io/github/SYNQfm/charybdis) | CDN log store | Jessica | [here](https://github.com/SYNQfm/charybdis/wiki)
[Calingi](https://github.com/SYNQfm/calingi) | [![CircleCI](https://circleci.com/gh/SYNQfm/calingi.svg?style=svg&circle-token=35f2b9d5ba20859dfee3af32129b8f746645f665)](https://circleci.com/gh/SYNQfm/calingi)| [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/calingi/badge.svg?t=AgvRqu)](https://coveralls.io/github/SYNQfm/calingi) | CDN log parse | Jessica | [here](https://github.com/SYNQfm/calingi/wiki)
[Aerico](https://github.com/SYNQfm/aerico) | [![CircleCI](https://circleci.com/gh/SYNQfm/aerico.svg?style=svg&circle-token=6bf28fed9b7e034017e2c7229049f774b3e80bc3)](https://circleci.com/gh/SYNQfm/aerico) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/aerico/badge.svg?t=Go4IJe)](https://coveralls.io/github/SYNQfm/aerico) | CLI Cleanup, Legacy -> New importer | Bruce | [here](https://github.com/SYNQfm/aerico/wiki)
[Anansi](https://github.com/SYNQfm/anansi) | [![CircleCI](https://circleci.com/gh/SYNQfm/anansi.svg?style=svg&circle-token=85d81001ef156fe3d431b47181bcc8bfa27bfb57)](https://circleci.com/gh/SYNQfm/anansi) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/anansi/badge.svg?t=QZb3mG)](https://coveralls.io/github/SYNQfm/anansi) | Metadata / Video quality analysis tool | Shan | [here](https://github.com/SYNQfm/anansi/wiki)
[Serpent](https://github.com/SYNQfm/serpent) | [![CircleCI](https://circleci.com/gh/SYNQfm/serpent.svg?style=svg&circle-token=72818c7c369b486bd9c73e132517731907e3e72e)](https://circleci.com/gh/SYNQfm/serpent) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/serpent/badge.svg?t=ztcRW1)](https://coveralls.io/github/SYNQfm/serpent) | Search Service | Shan |

__Frontend__

Name                                                        | Build | Code Coverage | Description  |  Maintainer(s) | Wiki Link
:-----------------------------------------------------------|------ | ------------- | ------------ | -------------- | -----------
[Duwende](https://github.com/SYNQfm/duwende) |[![CircleCI](https://circleci.com/gh/SYNQfm/duwende.svg?style=svg&circle-token=7824d007524d1618e7c8c702a6a2bdd7af0c914d)](https://circleci.com/gh/SYNQfm/duwende) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/duwende/badge.svg?branch=master&t=nBpAUi)](https://coveralls.io/github/SYNQfm/duwende?branch=master) | ReactJS based Dashboard for SYNQ | Fiona | 

__Shared Services__
 
Name                                                         | Build | Code Coverage |Description  |  Maintainer(s) |  Wiki Link  
:----------------------------------------------------------- | ------| --------------| ------------ | -------------- | ----------- 
[Imp](https://github.com/SYNQfm/imp) | N/A | N/A | DNS, Ansible | Glen, Bruce | [here](https://github.com/SYNQfm/imp/wiki) 
[Golang SDK](https://github.com/SYNQfm/SYNQ-Golang) | [![CircleCI](https://circleci.com/gh/SYNQfm/SYNQ-Golang.svg?style=svg)](https://circleci.com/gh/SYNQfm/SYNQ-Golang) | [![Coverage Status](https://coveralls.io/repos/github/SYNQfm/SYNQ-Golang/badge.svg?branch=master)](https://coveralls.io/github/SYNQfm/SYNQ-Golang?branch=master) | Shared Golang libraries | Bruce | 



Repo naming scheme is based on [legendary creatures](https://en.wikipedia.org/wiki/Lists_of_legendary_creatures), ideally matching the first (or more) letter(s) of the service "Search -> Serpent"

## Resources

[Technologies to Explore](https://github.com/SYNQfm/getting-started/wiki/Technologies-to-Explore) - if you read something cool, put it here    
[Useful Links](links.md)    
[General Wiki](https://github.com/SYNQfm/getting-started/wiki)
