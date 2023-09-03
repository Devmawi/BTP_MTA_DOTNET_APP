# Blazor Cloud Foundry App

Sample for demonstrating the deployment of a Blazor app to the cloud foundry environment.

## Prerequisites

* SAP BTP
* Cloud Foundry Runtime and Cloud Foundry Space
* NPM
* [Chocolatey](https://chocolatey.org/install)
    * `Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))`
* Cloud Foundry CLI
    * [Chocolatey](https://community.chocolatey.org/packages/cloudfoundry-cli)
    * [GitHub](https://github.com/cloudfoundry/cli/wiki/V8-CLI-Installation-Guide)
* [Make](https://community.chocolatey.org/packages/make)
* [npm install -g mbt](https://sap.github.io/cloud-mta-build-tool/download/)

## Useful commands

* `mbt build -t gen --mtar mta.tar`
* `cf install-plugin multiapps` or `cf install-plugin -r CF-Community "multiapps"`
* `cf deploy gen/mta.tar`, set optional `set DEBUG=1`

## Useful resources

* [CF CLI](https://docs.cloudfoundry.org/cf-cli/getting-started.html)
* [CF .NET Core Buildpack](https://docs.cloudfoundry.org/buildpacks/dotnet-core/index.html#pushing-apps)
* [MultiApps CF CLI Plugin](https://github.com/cloudfoundry/multiapps-cli-plugin)
* [MTA Module Types](https://help.sap.com/docs/btp/sap-business-technology-platform/modules#mta-module-types)