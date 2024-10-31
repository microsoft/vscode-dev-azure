# VS Code for the Web - Azure

VS Code for the Web - Azure is an Azure-specific environment for VS Code for Web.

<img width="1475" alt="image" src="https://github.com/microsoft/vscode-azurecontainerapps/assets/12476526/7b42685d-2e15-4ce4-afaf-c57d81455036">

## Entry points

1. Visit [https://insiders.vscode.dev/azure](https://insiders.vscode.dev/azure) directly to start using the product from scratch.
2. If you would like to start with a template, please visit [our preview version of the awesome-azd website](https://thankful-tree-067d73a10.5.azurestaticapps.net/). You can click on 'Try Template' to launch into vscode.dev/azure. The selected template will be automatically initialized in your vscode.dev/azure workspace. You can run `azd up` in the terminal to deploy the template to Azure.

<img width="1370" alt="image" src="https://github.com/microsoft/vscode-azurecontainerapps/assets/12476526/813a4494-cc1f-408d-8168-8be92feb2bcc">

## Using 

vscode.dev/azure will connect you to an Azure Cloud Shell instance. Once connected you can run, debug and deploy applications on vscode.dev/azure. Since the experience is using Azure Cloud Shell, you'll already be authenticated to Azure, and tools like the Azure CLI and AZD come preinstalled.

## Known Issues and Limitations  

1. The Docker daemon can’t run within Azure Cloud Shell. The Docker CLI is installed, however most operations (docker run, docker build) are not supported. 
2. Azure Cloud Shell instances that vscode.dev/azure connect to use Ehpemeral storage. Changes to the filesystem aren’t expected to persist between vscode.dev/azure sessions. 
3. A long initial loading time with a blank VS Code screen is expected. Please check whether there is a pop-up from VS Code asking you to sign in with Microsoft or GitHub. 

## Filing Issues 

Please create issues on this repository as you find them while using vscode.dev/azure.  

## How do I get access to the product? 

You will need to have an active Azure subscription that has our feature flag added to it. Please reach out to @meharida to send your **Azure subscription ID**.  

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
