# Jenkins-JIRA-Plugin

This repo supplies a Jenkinsfile that gets triggered upon status changes to issues in JIRA via a webhook (pre-configured in JIRA and Jenkins). Jenkins then uses the URL field in the JIRA issue (this is the URL to software that should be downloaded) and pulls the software from the web into a specificed folder inside a VM. If completed successfully, Jenkins updates the JIRA issue to be in 'Complete' status, if the build fails the JIRA issue moves to 'Blocked' status. Jenkins also adds comments to the JIRA issue throughout this process to keep users updated.
