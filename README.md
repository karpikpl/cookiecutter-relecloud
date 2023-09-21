# Cookiecutter Relecloud

## Deployment Options

|Feature| Django | FastAPI | Flask |
|---|---|---|---|
|**Deployment**|-|-|-|
|Deploys via AZD|✅|✅|✅|
|Deploys via Terraform|❌|❌|❌|
|Deploys via ACA|✅|✅|✅|
|Deploys with Azure App Service|✅|✅|✅|
|**Databases**|-|-|-|
|Azure ACA Postgres Plugin|✅|✅|✅|
|Azure Cosmos DB (Postgres Adapter)|✅|✅|✅|
|Azure Cosmos DB (MongoDB)|❌|🛠️|✅|
|Azure Postgres Flexible Server|✅|✅|✅|
|**Azure Add-ons**|-|-|-|
|Azure vNet|❌|❌|❌|
|Azure Secret KeyVault|✅|✅|✅|

|✅ (Developed)|🛠️ (In Development)|❌ (Currently Not Supported)|

## Deploying your cookiecutter template

1. Create a new folder
2. Create a virtual environment

```sh
python -m venv venv
source venv/bin/activate
```

2. Install necessary files

```sh
python -m pip install cruft packaging ruff black
```

3. Generate the project using this template

```sh
python -m cruft create https://github.com/kjaymiller/cookiecutter-relecloud
```

## Getting Updates from this Template

Cruft allows you to update your project with the latest changes from this template. To do so, run the following command:

```sh
cruft update
```

## Running your Deployment via DevContainer/Github Codespaces

This template is designed to work with DevContainers and GitHub Codespaces. You can deploy the Github Codespaces instance by clicking the green code button and creating a new codespace.

To deploy the dev container locally you can do so with a compatible code editor like Visual Studio Code.

## Deploy your template to Azure

These templates are configured to deploy to Microsoft Azure via the Azure Developer CLI. You can deploy your project immediately using `azd up`

## Deployed Project Examples

### Django

----------

- [Django Postgres - Flexible Server Azure Container Apps](https://github.com/Azure-Samples/django-postgres-flexible-aca)
- [Django Postgres - Flexible Server Azure App Service](https://github.com/Azure-Samples/django-postgres-flexible-appservice)
- [Django CosmosDB Postgres Adapter Azure Container Apps](https://github.com/Azure-Samples/django-cosmos-postgres-aca)
- [Django CosmosDB Postgres Adapter Azure App Service](https://github.com/Azure-Samples/django-cosmos-postgres-appservice)
- [Django Azure Container Apps Postgres Addon Azure Container Apps](https://github.com/Azure-Samples/django-postgres-addon-aca)

### FastAPI

----------

- [FastAPI Postgres - Flexible Server Azure Container Apps](https://github.com/Azure-Samples/fastapi-postgres-flexible-aca)
- [FastAPI Postgres - Flexible Server Azure App Service](https://github.com/Azure-Samples/fastapi-postgres-flexible-appservice)
- [FastAPI CosmosDB Postgres Adapter Azure Container Apps](https://github.com/Azure-Samples/fastapi-cosmos-postgres-aca)
- [FastAPI CosmosDB Postgres Adapter Azure App Service](https://github.com/Azure-Samples/fastapi-cosmos-postgres-appservice)
- [FastAPI Azure Container Apps Postgres Addon Azure Container Apps](https://github.com/Azure-Samples/fastapi-postgres-addon-aca)

### Flask

----------

- [Flask Postgres - Flexible Server Azure Container Apps](https://github.com/Azure-Samples/flask-postgres-flexible-aca)
- [Flask Postgres - Flexible Server Azure App Service](https://github.com/Azure-Samples/flask-postgres-flexible-appservice)
- [Flask CosmosDB Postgres Adapter Azure Container Apps](https://github.com/Azure-Samples/flask-cosmos-postgres-aca)
- [Flask CosmosDB Postgres Adapter Azure App Service](https://github.com/Azure-Samples/flask-cosmos-postgres-appservice)
- [Flask Azure Container Apps Postgres Addon Azure Container Apps](https://github.com/Azure-Samples/flask-postgres-addon-aca)
- [Flask CosmosDB - MongoDB Adapter Azure Container Apps](https://github.com/Azure-Samples/flask-cosmos-mongodb-aca)
- [Flask CosmosDB - MongoDB Adapter Azure App Service](https://github.com/Azure-Samples/flask-cosmos-mongodb-appservice)
