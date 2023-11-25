# Sample Salesforce Workflows

This is a collection of Github Workflow Actions meant to support Salesforce projects.

## Setup

These actions assume you have a working dev hub connection that you can use as a repository secret. Use the following instructions to get the secret into place. Please understand that the key allows anyone with it to log into the deb hub org as the user who the connection is connected to. [Please make sure you understand your choices](https://developer.salesforce.com/docs/atlas.en-us.sfdx_dev.meta/sfdx_dev/sfdx_setup_add_users.htm#sfdx_setup_add_users).

1. On your local machine connect to the devhub you wish to use.
2. Run `sf org display -o [your devhub alias] --verbose`
3. Find the section labeled `Sfdx Auth Url`. You'll need that value as your secret.
4. In your Github repo's settings, find Secrets and Variables, and open the subsection for Actions.
5. Create a new repository secret called `DEVHUB_SFDX_URL`. Copy the secret value you found in step 3.
