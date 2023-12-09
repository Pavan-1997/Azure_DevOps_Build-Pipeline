# Azure DevOps Build Pipeline

## Steps to set the infrastructure
- Login to VSCode or any other IDE of your choice
- Download the application code
- Create a project in Azure DevOps and push the code by running the below commands on VSCode:
  ```
  git remote add origin $YOURAZUREREPO
  git push -u origin all
  ```
  Note: Make sure to update your Azure repo in the above command

- Go to the Azure Portal and Create the Azure App Service by following the instructions in the video

- Implement the build pipeline using the classic editor

- Understand the use of service connection and service principal

![image](https://github.com/Pavan-1997/Azure_DevOps_Build-Pipeline/assets/32020205/46352809-cc2e-473d-b1c4-39f1940266e2)

Note: You must set the app settings WEBSITE_DYNAMIC_CACHE=0 and WEBSITE_LOCAL_CACHE_OPTION=Never to disable all file caching

