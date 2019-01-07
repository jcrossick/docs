---
title: Install the Deploy CLI Tool
description: Learn how to install the Deploy CLI tool.
topics:
  - extensions
  - deploy-cli
contentType:
  - how-to
useCase: extensibility-extensions
---
# Install the Deploy CLI Tool

## Prerequisites

For this tool to function it must be authorized to the Auth0 Management API. You can do this by creating an application in your Auth0 service that has access to the management API with the following scopes before.

### Scopes
  * read:client_grants
  * create:client_grants
  * delete:client_grants
  * update:client_grants
  * read:clients
  * update:clients
  * delete:clients
  * create:clients
  * read:client_keys
  * update:client_keys
  * delete:client_keys
  * create:client_keys
  * read:connections
  * update:connections
  * delete:connections
  * create:connections
  * read:resource_servers
  * update:resource_servers
  * delete:resource_servers
  * create:resource_servers
  * read:rules
  * update:rules
  * delete:rules
  * create:rules
  * read:rules_configs
  * update:rules_configs
  * delete:rules_configs
  * read:email_provider
  * update:email_provider
  * delete:email_provider
  * create:email_provider
  * read:tenant_settings
  * update:tenant_settings
  * read:grants
  * delete:grants
  * read:guardian_factors
  * update:guardian_factors
  * read:email_templates
  * create:email_templates
  * update:email_templates

Use the [Auth0 Deploy CLI Extension](https://github.com/auth0-extensions/auth0-deploy-cli-extension/blob/master/README.md) to create the application. 

## Install the tool using `bash`

```
bash
npm i -g auth0-deploy-cli
```

## Alternative installation method

To create the client application manually: 

1. Log into your dashboard.
   1.  Click the applications tab.
   1.  Click the **Create Application** button.
       1.  Name it something like **Deploy Client**.
       1.  Select **Machine-to-Machine** as the application type.
       1.  Click **Create**.
   1.  Use the **Select an API** dropdown to choose: **Auth0 Management API**.
   1.  Select the [scopes](#scopes) as defined above.
   1.  Click **Authorize**.

## Keep reading

* [Incorporate Deploy CLI into Build Environment](/extensions/deploy-cli/guides/incorporate-deploy-cli-into-build-environment)
* [Call Deploy CLI Tool Programmatically](/extensions/deploy-cli/guides/call-deploy-cli-programmatically)
* [Deploy CLI Tool Options](/extensions/deploy-cli/references/deploy-cli-options)
* [Test Deploy CLI Operations Locally](/extensions/deploy-cli/guides/test-locally)* [Import/Export Tenant Configuration to a Directory Structure](extensions/deploy-cli/guides/import-export-directory-structure)
* [Import/Export Tenant Configuration to a YAML File](/extensions/deploy-cli/guides/import-export-yaml-file)