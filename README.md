# VS Code for the Web - Azure

VS Code for the Web - Azure is an Azure-specific environment for VS Code for Web that leverages Azure Cloud Shell.

In a nutshell, it's VS Code running from within your Azure Cloud Shell. You can run, debug and deploy Azure applications from the browser. Common Azure tools such as the Azure CLI, Python, and azd are pre-installed.

<img width="1475" alt="image" src="https://github.com/microsoft/vscode-azurecontainerapps/assets/12476526/7b42685d-2e15-4ce4-afaf-c57d81455036">

## Using

There are two main ways to use VS Code for the Web - Azure. Either start with an azd template, or start from scratch with an empty workspace.

### azd template

[What is azd?](https://learn.microsoft.com/en-us/azure/developer/azure-developer-cli/)

If you would like to start with an azd template, please visit [our preview version of the awesome-azd website](https://aka.ms/vscode-dev-azd-templates). You can click on 'Try Template' to launch into vscode.dev/azure. The selected azd template will be automatically initialized in your VS Code for the Web - Azure workspace. You can run `azd up` in the terminal to deploy the template to Azure. 

<img width="1370" alt="image" src="https://github.com/microsoft/vscode-azurecontainerapps/assets/12476526/813a4494-cc1f-408d-8168-8be92feb2bcc">

### Starting from scratch

You can also use VS Code for the Web - Azure without using an azd template. This will open a blank workspace. To do this, go directly to https://insiders.vscode.dev/azure.

### Logging in

Whether coming from a template, or starting from scratch, once you reach https://insiders.vscode.dev/azure, you'll be prompted to login with your Azure account. Select "Allow". Make sure to sign in with the account that contains the subscription you provided when signing up.

<img width="608" alt="Image" src="https://github.com/user-attachments/assets/c12b97cf-e182-4cd0-8fe6-b4b1ac42d7d6" />
<img width="676" alt="Image" src="https://github.com/user-attachments/assets/3fb3fb56-e282-4f49-b9b0-7f754daf8ae6" />

If your account belongs to more than one tenant, you'll be asked to select one. Make sure to select the tenant that contains the subscription you provided when signing up.

<img width="680" alt="Image" src="https://github.com/user-attachments/assets/c0477392-0d98-49e6-a258-2c50be8a036b" />

After signing in and selecting a tenant (if required), you'll start connecting to an Azure Cloud Shell instance. If at this point you see an error saying "Access denied. Account and tenant don't contain an allowed subscription." it means you haven't been granted access to the private preview. If you see this error and believe it's a mistake, please file an issue and label it as a product access bug.

## Known Issues and Limitations  

1. Azure Cloud Shell instances that vscode.dev/azure connect to use Ehpemeral storage. This means changes to the filesystem aren’t expected to persist between different vscode.dev/azure sessions.
2. A long initial loading time is expected. This could be up to 60 seconds.

## Troubleshooting

### Account type prompt issue

If you see a prompt asking "What type of account did you use to start this tunnel?" then it's likely that you're on vscode.dev/azure and not **insiders**.vscode.dev/azure. Currently this product is only available on Insiders. To fix this, navigate to https://insiders.vscode.dev/azure. ![image](https://github.com/user-attachments/assets/eb8487fe-c968-4cdb-b28d-c853d71ebcf8)

### Connection issue

If you're unable to connect to insiders.vscode.dev/azure, you can usually fix it by resetting your Azure Cloud Shell. This can be done from the Azure Portal.

1. Open Cloud Shell in the Azure Portal using the button in the top right corner.

![Open Azure Cloud Shell in the Azure Portal](https://github.com/user-attachments/assets/290ac148-8482-4ea6-82ab-3ab7733b9881)

2. Next, in the Settings dropdown, select Reset User Settings.

![Reset user settings](https://github.com/user-attachments/assets/8721515f-00b3-4447-83f1-5fba9bdbbad9)

3. Once finished you should see this screen.

![image](https://github.com/user-attachments/assets/d4dadf26-670e-4803-93eb-f0139dd8db64)

### Gathering logs

The extension logs will help us diagnose any issues with vscode.dev/azure. You can access them by going to the Output view, then selecting the "VS Code for the Web - Azure" output channel.

<img width="522" alt="image" src="https://github.com/user-attachments/assets/5fdbc41c-6446-4739-a467-eb408224a7e5" />

<img width="385" alt="image" src="https://github.com/user-attachments/assets/8604d173-0e93-4541-ad13-ee4c99df4b25" />

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
