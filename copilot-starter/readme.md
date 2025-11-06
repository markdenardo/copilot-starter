# project launch instructions
to start this project do the following:
1. install requirements in bash
```pip install -r requirements.txt```
2. install azure extentions 
3. create an azure cli terminal
through the azure tab in the tools tab, create an azure cli resource
the cli will open as an az dev below your bash script
3. login to azure cli and follow the prompts
```azd login```
4. initialize project
```azd init```
5. use a unique name using the convention ```user-date-app_name```
6. update .env credentials
edit ```.azure/user-date-app_name/.env```
```
AZD_ALLOW_NON_EMPTY_FOLDER="true"
AZURE_ENV_NAME="user-date-app_name"
AZURE_EXISTING_AIPROJECT_ENDPOINT="https://name-of-resource.openai.azure.com/"
AZURE_EXISTING_AIPROJECT_RESOURCE_ID="your-resource-id-here"
AZURE_LOCATION="name-of-location"
AZURE_SUBSCRIPTION_ID="your-subscription-id-here"
```
7. deploy
```azd up```
8. test deployment link provided in the cli message and go to azure resource link
9. delete resource
```azd down```
