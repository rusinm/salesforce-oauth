salesforce-oauth
================

This examples shows how to connect to Salesforce using OAuth.

Step 1: log in to Salesforce
Step 2: go to Setup. enter 'apps' in the search filter on the left and click Create -> Apps
Step 3: click new in the Connected Apps section
Step 4: fill in the name and contact email. check Enable OAuth Settings. callback url will be http://localhost:8081/oauth2callback. from Selected OAuth Scopes choose Full Access and save.
Step 5: after saving you will see app info. copy Consumer Key to sfdc.oauth.consumerKey of common.properties. do the same for Consumer Secret
Step 6: run mule app and go to http://localhost:8081 in the browser
Step 7: Success: output of the console should contain sth like:

INFO  2014-06-27 12:31:42,410 [batch-job-salesforce-oauthBatch1-work-manager.02] org.mule.api.processor.LoggerMessageProcessor: contact processed: {LastModifiedDate=2014-05-08T09:05:18.000Z, Id=0032000001DpkrBAAR, type=Contact, LastName=Ripley}
INFO  2014-06-27 12:31:42,412 [batch-job-salesforce-oauthBatch1-work-manager.02] org.mule.api.processor.LoggerMessageProcessor: contact processed: {LastModifiedDate=2014-05-08T09:05:18.000Z, Id=0032000001DpkrCAAR, type=Contact, LastName=D'Cruz}
I

