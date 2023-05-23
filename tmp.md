```
az ad sp create-for-rbac --name "azureml-principal-poyu" --role contributor \
                         --scopes /subscriptions/095c17da-056e-43f2-8d52-a30d1bdb6423/resourceGroups/MLOps \
                         --sdk-auth
```