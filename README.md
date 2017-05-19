# Spryker Demo Shop on Azure
ARM Template to deploy the Spryker demo shop on Azure using managed services. This includes App Service on Linux, Azure Redis Cache, Azure Postgresql, and an Elastic Search Cluster.

# Deplyoment
```
$ az group create -n myrg -l northeurope
$ az group deployment create -g myrg --mode Complete --template-file azuredeploy.json --parameters @azuredeploy.parameters.json
