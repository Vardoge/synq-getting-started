## Deployment (for Obaku)

* Deploy to production happens Tuesday at 17:00 - 20:00 CET/CEST if there are changes to be deployed
* Only officialy created "releases" should be deployed to production
* Out of band deploys should only happen for critical outages or major security holes
* Anyone should be able to deploy
* Our goal is continuous deployment so aim for more automation

### Deploy Procedures

We will create release notes for the specific workspace, and copy the deploy procedures from the previous release to the latest release.  Thus, we don't have a single "deploy" doc, but more of a living procedure that lives in our release notes.

__Core Service (Obaku)__ - Example releases on [2017-05-09](https://github.com/SYNQfm/obaku/releases/tag/2017-05-09) and [2017-07-11](https://github.com/SYNQfm/obaku/releases/tag/2017-07-11)    
__Thumbnail__ - This lives inside Core, and is upgraded [2017-06-06](https://github.com/SYNQfm/obaku/releases/tag/2017-06-06).  Note, that there's an effort to migrate this to its own [repo](https://github.com/SYNQfm/tylwythteg) which will result in separate deploy procedures    
__Streamer__ - Example release [v0.3.0](https://github.com/SYNQfm/streamer/releases/tag/v0.3.0)    

### Post Deploy Testing

* [Guideline](https://github.com/SYNQfm/obaku/wiki/Guide:-Testing-New-Changes-to-Obaku-and-Post-Deployment-Tests)

### Versioning

Current we have two models, one is "date" based, and one is "version" based.  We still need to finalize on one and standardize it.
