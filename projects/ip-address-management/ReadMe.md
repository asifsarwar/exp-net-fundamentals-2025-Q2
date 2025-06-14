## Deploy Windows Server

```sh
az deployment group create --resource-group net-fun-bootcamp --template-file template.bicep --parameters @parameters.json
```