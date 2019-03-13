# WARNING

**Using the "Deploy to Azure" button will allow you to deploy this Integration (which is an Azure Functions App essentially) to an Azure Resource Group of your choice. Please be aware that during the deployment process an App Service Instance will be created which uses the "Basic" App Service Plan as the minimum Service Plan. This App Service Plan is associated with a monthly subscription cost. More info can be found [here](https://azure.microsoft.com/en-us/pricing/details/app-service/windows/). The reason for using the "Basic" App Service Plan as a minimum is the requirement to keep the Azure Function App running constantly because it listens to incoming MQTT packets from the The Things Network Data API. Functions Apps running on the "Consumption" Plan will be shut down automatically after 10 minutes and the connection to the Data API of TTN will be lost. Running Functions Apps on the "Free" and "Shared" App Service Plans is currently not possible. So, you have been warned! If you're still eager to try this Integration, hit the "Deploy to Azure" button below. Have fun!**
 
[![Deploy to Azure](https://azuredeploy.net/deploybutton.png)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fjsiebert%2FTTNAzureBridge%2Fmaster%2Fazuredeploy.json)