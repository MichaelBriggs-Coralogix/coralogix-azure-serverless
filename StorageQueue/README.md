# Azure Storage Queue Trigger Function for Coralogix

Coralogix provides a seamless integration with ``Azure`` cloud so you can send your logs from anywhere and parse them according to your needs.

The Azure Storage Queue integration allows parsing of queue messages in JSON format. Other format messages will not be processed and submitted to the Coralogix platform.

## Prerequisites

* An Azure account with an active subscription.

## Azure Resource Manager Template Deployment

The Storage Queue integration can be deployed by clicking the link below and signing into your Azure account:
[Deploy to Azure](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fcoralogix%2Fcoralogix-azure-serverless%2FFEAT%2FARM-Deploy%2FStorageQueue%2FARM%2FStorageQueue.json)

## Guide

**Subscription** - The Azure Subscription into which you wish to deploy the integration.

**Resource Group** - The Resource Group into which you wish to deploy the integration.

**Coralogix URL** - The logs API URL for your Coralogix region.

**Coralogix Private Key** – Can be found in your Coralogix account under Settings -> Send your logs. It is located in the upper left corner.

**Coralogix Application** – A mandatory metadata field that is sent with each log and helps to classify it. (Default: Azure)

**Coralogix Subsystem** – A mandatory metadata field that is sent with each log and helps to classify it. (Default: StorageQueue)

**Storage Queue Connect String** - The Primary Connect String of the Storage Account containing the Storage Queue to be monitored.

**Storage Queue Name** - The name of the Storage Queue to be monitored.
