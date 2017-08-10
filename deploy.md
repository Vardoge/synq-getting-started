## Deployment (for Obaku)

* Releases are tagged and finalized on Mondays by 15:00 local Oslo time
* Deploy to production happens every Tuesday at 13:00-16:00 local Oslo time
* Only officialy created "releases" can be deployed to production
* Deploys should be done with scripts and avoid manual intervention or work
* Out of band deploys should only happen for critical outages or major security holes
* Anyone should be able to deploy
* Our goal is continuous deployment and moving the deploys to monday as they get leaner

### Deploy Procedures

We will create release notes for the specific workspace, and copy the deploy procedures from the previous release to the latest release.  Thus, we don't have a single "deploy" doc, but more of a living procedure that lives in our release notes.

__Core Service (Obaku)__ - Example Release on [2017-05-09](https://github.com/SYNQfm/obaku/releases/tag/2017-05-09) and [2017-07-11](https://github.com/SYNQfm/obaku/releases/tag/2017-07-11)    
__Thumbnail__ - This lives inside the Obaku workspace, but it runs on a separate server, so its upgrade will be described in the Obaku release notes.    
__Streamer__ - Release for [v0.3.0](https://github.com/SYNQfm/streamer/releases/tag/v0.3.0)    

[Post Deploying Testing Template](https://github.com/SYNQfm/obaku/wiki/Post-Deployment-Testing-Template)    

### Versioning

Current we have two models, one is "date" based, and one is "version" based.  We still need to finalize on one and standardize it.