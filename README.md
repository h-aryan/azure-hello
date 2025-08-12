# Basic Azure Python Web App

## Local Development

```bash
pip install -r requirements.txt
python app.py
```

## Deploy to Azure

1. Create a resource group:
   ```bash
   az group create --name myResourceGroup --location eastus
   ```

2. Deploy resources:
   ```bash
   az deployment group create --resource-group myResourceGroup --template-file azuredeploy.json
   ```

3. Deploy your code using Azure Portal or GitHub Actions.

## Files

- `app.py`: Basic Flask app
- `requirements.txt`: Dependencies
- `azuredeploy.json`: ARM template for Azure App Service
