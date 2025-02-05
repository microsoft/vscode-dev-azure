# VS Code for the Web - Azure

VS Code for the Web - Azure is an Azure-specific environment for VS Code for Web that leverages Azure Cloud Shell.

In a nutshell, it's VS Code running from within your Azure Cloud Shell. You can run, debug and deploy Azure applications from the browser. Common Azure tools such as the Azure CLI, Python, and azd are pre-installed.

<img width="1475" alt="image" src="https://github.com/microsoft/vscode-azurecontainerapps/assets/12476526/7b42685d-2e15-4ce4-afaf-c57d81455036">

## How do I get access to the product? 

You will need to have an active Azure subscription that has our feature flag added to it. Please fill out the form at this link to request access: https://aka.ms/VSCodefortheWebAzure

## Entry points

There are two main ways to use VS Code for the Web - Azure. The first is starting from an azd template from [this template website (https://aka.ms/vscode-dev-azd-templates)](https://aka.ms/vscode-dev-azd-templates). [What is azd?](https://learn.microsoft.com/en-us/azure/developer/azure-developer-cli/). 

1. If you would like to start with an azd template, please visit [our preview version of the awesome-azd website](https://aka.ms/vscode-dev-azd-templates). You can click on 'Try Template' to launch into vscode.dev/azure. The selected azd template will be automatically initialized in your vscode.dev/azure workspace. You can run `azd up` in the terminal to deploy the template to Azure.
2. Visit [https://insiders.vscode.dev/azure](https://insiders.vscode.dev/azure) directly to start using the product from scratch.

<img width="1370" alt="image" src="https://github.com/microsoft/vscode-azurecontainerapps/assets/12476526/813a4494-cc1f-408d-8168-8be92feb2bcc">

## Using

### azd template

Whether coming from a template, or starting from scratch, once you reach https://insiders.vscode.dev/azure, you'll be prompted to login with your Azure account. Select "Allow". Make sure to sign in with the account that contains the subscription you provided when signing up.

### Starting from scratch

<img width="608" alt="Image" src="https://github.com/user-attachments/assets/c12b97cf-e182-4cd0-8fe6-b4b1ac42d7d6" />
<img width="676" alt="Image" src="https://github.com/user-attachments/assets/3fb3fb56-e282-4f49-b9b0-7f754daf8ae6" />

If your account belongs to more than one tenant, you'll be asked to select one. Make sure to select the tenant that contains the subscription you provided when signing up.

<img width="680" alt="Image" src="https://github.com/user-attachments/assets/c0477392-0d98-49e6-a258-2c50be8a036b" />

After signing in and selecting a tenant (if required), you'll start connecting to an Azure Cloud Shell instance. If at this point you see an error saying "No subscription found with Cloud Shell feature registered." it means you haven't been granted access to the private preview. If you see this error and believe it's a mistake, please file an issue and label it as a product access bug.

## Known Issues and Limitations  

1. Azure Cloud Shell instances that vscode.dev/azure connect to use Ehpemeral storage. This means changes to the filesystem aren’t expected to persist between different vscode.dev/azure sessions.
2. A long initial loading time is expected.

## Filing Issues 

Please create issues on this repository as you find them while using vscode.dev/azure. The more detail the better. If possible, please include logs from the "VS Code for the Web - Azure" output channel.

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
