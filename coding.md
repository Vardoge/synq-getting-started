# Coding Culture

This document describes our development philosophy and the reasoning behind the way we do certain things and show very specific examples of how we live by our philosophy.  Anyone can suggest changes to this document, but its good to read this first to understand the why on our process

## Our Mission

`To deliver business value quickly by shipping production code continuously`

## How and why we do it

In order to accomplish our goal, we do the below things.  Click on each item to see more details


What   | Reasoning | Tooling | Category
:------- | ----- | --------- | -------
[Tight CI/CD](ci.md) | The way we can ship the code quickly and confidently | GithHub, CircleCI, Nanobox + Digital Ocean or Heroku | CI/CD
[High code coverage](ci.md) | CI is useless without good quality coverage, and we can't ship to production quickly if we are confident we won't break everything | CircleCI, Coveralls | CI/CD
[Atomic (or close) PRs](code.md) | Pushing smaller changes reduces chance of breakage but also delivering it fast | GitHub | Code
[Refactor constantly](code.md) | Code debt slows us down and to counter our fast PR turnaround | GitHub | Code
[Automated System/UI Testing](auto.md) | Once code is in production, is it really working?  Running things like Runscope against the API gives us confidence that new changes didn't mess up prod | CircleCI, Runscope, GhostInspector, TestLodge | Code
[Peer Reviews](docs.md) | Make sure the code meets our needs, sharing knowledge | GitHub, Slack | Docs
[Good documentation](docs.md) | moving quickly means we work on a lot of different things, coming back to it later or having another teammmate look at it, they need to know | GitHub Markdown, Wiki, Stoplight | Docs
[DevOps Culture](auto.md) | Everyone should know how stuff runs and keep an eye that services are working as expected | Slack, Runscope, PagerDuty, StatusPages | DevOps