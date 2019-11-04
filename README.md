## Azure

```bash
brew update && brew install azure-cli
az extension add --name azure-devops

az login
az devops -h

az repos -h
az repos list --org https://dev.azure.com/bcircle-development

az pipelines -h
az pipelines show -h
az pipelines show --org https://dev.azure.com/bcircle-development  --project inflex-monitor --id 5
az pipelines list --org https://dev.azure.com/bcircle-development  --project inflex-monitor --output yaml

az pipelines build --project inflex-monitor  --id 5
az pipelines queue list --org https://dev.azure.com/bcircle-development --project inflex-monitor
```