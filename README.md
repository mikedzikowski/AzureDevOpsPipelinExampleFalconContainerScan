# AzureDevOpsPipelineExampleFalconContainerScan
An example Azure DevOps Pipeline that will scan a container image and conditionally push the image to an Azure Container Registry based on Image Assessment API policy response.

This pipeline leverages the FCS IaC tool to scan a DevOps repo, Falcon Cloud Security Image Assesment policies and Azure Container Registries to scan a container images and based on an API response. Based on the API response the pipeline will conditionally build the image in a registry. By integrating these tools into a pipeline, developers will have the opportunity to address any security issues before deploying updates into their containers. 

API Response True - Block Image build

![alt text](/images/failbuild.png)


API Response False - Allow Image build

![alt text](/images/allowbuild.png)
