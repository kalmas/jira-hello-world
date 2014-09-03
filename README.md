jira-hello-world
================

Just a trivial example of a plugin for an OnDemand instance of JIRA using Atlassian Connect. Based on [this tutorial](https://developer.atlassian.com/static/connect/docs/guides/getting-started.html).

To Deploy
---------

1. Modify descriptor file (public/atlassian-connect.json)
  - "key" must be unique
  - "baseUrl" should be your host. Must be served over HTTPS
2. Modify path to all.js script in public/atlassian-connect.json, should be "//{Your OnDemand Host}}/atlassian-connect/all.js"
3. Start app
4. Go to Atlassian Marketplace and create an Add-On https://marketplace.atlassian.com/manage/plugins/create
  - select "Provide a URL to your artifact" option and provide url to your atlassian-connect.json
  - ALL the metadata!
5. Install add-on in Univeral Plugin Manager (Cog Icon > Add-Ons > Manage Add-Ons > Upload Add-On)