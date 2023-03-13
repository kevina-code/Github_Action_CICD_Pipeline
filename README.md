# Github_Actions_Pipeline
This is custom CI/CD pipeline script I wrote that validates/deploys to a Salesforce sandbox.

It validates upon pull_request, and deploys upon merge/commit to master

To use this script, you will need to set the following secrets in the repo:
1. SANDBOX_USERNAME
2. SANDBOX_INSTANCE_URL
3. SANDBOX_CLIENTID

You will also either need to delete the SLACK blocks from the script, or configure your own Slack webhooks to be parsed by the script so that your specified Slack channels can be notified.
