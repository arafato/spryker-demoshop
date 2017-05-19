# Spryker Demoshop on Azure
ARM Template to deploy the Spryker demo shop on Azure using managed services (except ElastiSearch). This includes App Service on Linux, Azure Redis Cache, Azure Postgresql, and an Elastic Search Cluster.

The Demoshop is based on the Spryker Commerce Framework http://spryker.com/

# Deployment
```
$ az group create -n myrg -l northeurope
$ az group deployment create -g myrg --mode Incremental --template-file azuredeploy.json --parameters @azuredeploy.parameters.json
```

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Farafato%2Fspryker-demoshop%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>