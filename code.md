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
  
### Supporting Prospects/Customers

* We use [Zendesk](https://synqsupport.zendesk.com) for support email and the [synq-onboarding](https://synq-onboarding.slack.com) slack channel to help customers.
* We use Hubspot to track our customers and various interactions and converting our leads into signed deals.

## Best Practices

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
