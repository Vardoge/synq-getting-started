### Test / Deploy / Run

* We use [CircleCI](https://circleci.com/dashboard) for Continous Integration
* We use [Coveralls](https://coveralls.io/) to monitor test coverage
* Aim for continuous deployment. Maintainers determine the release cadence but changes _should_ be deployed at least once a week
  * Some services use [Heroku](https://dashboard.heroku.com/teams/synqfm/apps) with automatic deploys on changes to `master`
  * Some services use [Nanobox](https://dashboard.nanobox.io/)
* We use [Runscope](https://www.runscope.com/radar/si8c3oxplpmd) to continuously monitor our APIs 
* We use [PagerDuty](https://app.pagerduty.com/) to manage on call and alerts
* We use [StatusPage](https://manage.statuspage.io/pages/x9f990zglm69) to communicate public API [status](https://synq.statuspage.io/) information to customers

