# Github_Actions_Pipeline
This is custom CI/CD pipeline script that validates/deploys to a Salesforce sandbox.

Prereqs: 
1. A generic API User has been created in your Salesforce org
2. A Connected App with elevated permissions has been created in your Salesforce org

It validates upon pull_request, and deploys upon merge/commit to master

To implement, you will need to set the following secrets in the repo:
1. SANDBOX_USERNAME (ex: apiuser@mycompany.com)
2. SANDBOX_INSTANCE_URL (ex: mycompany--staging.my.salesforce.com
3. SANDBOX_CLIENTID (the client Id of the Connected App you created in Salesforce)
