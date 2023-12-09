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

## Structure of Azure DevOps build Pipeline

*  A trigger tells a Pipeline to run. It could be CI or Scheduled, manual(if not specified), or after another build finishes.
*  A pipeline is made up of one or more stages. A pipeline can deploy to one or more environments.
*  A stage organizes jobs in a pipeline, and each stage can have one or more jobs.
*  Each job runs on one agent, such as Ubuntu, Windows, macOS, etc. A job can also be agentless.
*  Each agent runs a job that contains one or more steps.
*  A step can be a task or script and is the smallest building block of a pipeline.
*  A task is a pre-packaged script that performs an action, such as invoking a REST API or publishing a build artifact.
*  An artifact is a collection of files or packages published by a run.
