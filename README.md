# README #

Microsoft Azure DevCamp Hands On Lab

Node js and azure service integration

### What is this repository for? ###

* Node js and azure service integration

### What's Inside ###

* Integrate the API
* Add a caching layer
* Write images to Azure Blob storage
* Take an anonymous application and add user authentication via AzureAD.
* Query data from the Microsoft Graph.
* Manipulate data in the Microsoft Graph.

### Who do I talk to? ###

* davidalfasunarna@gmail.com

### Getting Started ###

* I am using vscode 
* Create .vscode/launch.json and paste the code

```json
{
    "version": "0.2.0",
    "configurations": [
    
        {
            "type": "node",
            "request": "launch",
            "name": "Launch Program",
            "program": "${workspaceFolder}/app.js",
            "env": {
                "NODE_ENV": "development",
                "INCIDENT_API_URL": "[azure_api_url]",
                "REDISCACHE_HOSTNAME": "[azure_api_hostname]",
                "REDISCACHE_PRIMARY_KEY": "[azure_redis]",
                "REDISCACHE_PORT": "6379",
                "REDISCACHE_SSLPORT": "6380",
                "AZURE_STORAGE_ACCOUNT": "[azure_storage_account]",
                "AZURE_STORAGE_ACCESS_KEY": "[azure_storage_account_access_key]",
                "AZURE_STORAGE_BLOB_CONTAINER": "images",
                "AZURE_STORAGE_QUEUE": "thumbnails",
                "AAD_RETURN_URL": "[oauth_api]",
                "AAD_CLIENT_ID": "[app_dev_client_id]",
                "AAD_CLIENT_SECRET": "[app_dev_client_secret]"
            }
        }
    ]
}
``` 
* mpm install
