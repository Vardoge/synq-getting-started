# Coding Culture

This document describes our development philosophy and the reasoning behind the way we do certain things and show very specific examples of how we live by our philosophy.  Anyone can suggest changes to this document, but its good to read this first to understand the why on our process

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